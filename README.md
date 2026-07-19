# 📊 Global Life Expectancy & Health Determinants Analysis

An exploratory data analysis (EDA) and predictive modeling project that examines the relationships between **Life Expectancy** and various health, economic, and developmental indicators worldwide. The analysis utilizes historical data from the **World Health Organization (WHO)** spanning from 2000 to 2015.

---

## 📌 Project Overview
* **Dataset Size:** 2,938 rows and 22 features.
* **Core Objective:** Investigate socioeconomic factors driving global health disparities between developing and developed nations, and build a baseline predictive model for life expectancy.

---

## ⚙️ Methodology & Key Findings

### 1. Data Cleaning & Preprocessing
* **Missing Values Handling:** Missing data percentages varied across features (e.g., `GDP` at 15.25%, `BMI` at 1.15%). Missing entries for features like `BMI`, `Schooling`, and `GDP` were handled using country-specific imputation and median/mean strategies.
* **Feature Pruning:** The `Population` column was dropped due to a high ratio of missing values (exceeding 22%).
* **Temporal Formatting:** The `Year` attribute was converted to a uniform `datetime` format to ensure seamless time-series continuity.

### 2. Descriptive Statistics
* **Global Average:** The overall global life expectancy stands at **69 years** (averaging 79 years for developed nations vs. 67 years for developing nations).
* **Continental Insights:** **Europe** recorded the highest average life expectancy (**77.4 years**), whereas **Africa** recorded the lowest (**58.6 years**).
* **Economic Correlation:** High-income countries with advanced education metrics (e.g., Australia, Austria) consistently topped the charts with life expectancies exceeding 81 years.

### 3. Aggregation & Query Highlights
* **Top Performing Countries:** Japan (82.54), Sweden (82.52), and Iceland (82.44).
* **Lowest Performing Countries:** Angola (49.02), Malawi (49.89), and Chad (50.39).
* **Historical Growth:** Global life expectancy showed steady progression, climbing from 66.7 years in 2000 to 71.6 years in 2015.
* **Developmental Success Stories:** Significant multi-year leaps were observed in countries like **Zimbabwe (+21 years)** and **Eritrea (+19.4 years)**.

### 4. Data Visualization
The analysis incorporates comprehensive visualizations including:
1. **Distribution & Comparison:** Histograms and boxplots comparing life expectancy frequency across developed vs. developing nations.
2. **Time-Series Analysis:** Trends showing immunization coverage (Hepatitis B, Polio, Diphtheria) over the 15-year span.
3. **Correlation Matrices:** Heatmaps highlighting the strong positive correlation between education (`Schooling`), income composition, and life expectancy.

### 5. Advanced Statistical Testing & Modeling
* **Correlation Coefficients:** Pearson and Spearman tests confirmed statistically significant positive linear and monotonic relationships between GDP and Life Expectancy.
* **Hypothesis Testing (T-test):** An independent T-test confirmed a statistically significant gap of **12.1 years** in favor of developed countries.
* **Predictive Modeling:** A baseline **Linear Regression** model was trained using 3 key features (`GDP`, `BMI`, `Schooling`), achieving a solid performance metric of **$R^2 = 0.618$**.

---

