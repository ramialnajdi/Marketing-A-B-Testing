# **Marketing A/B Testing Analysis**

## **Overview**
This project analyzes a marketing dataset to evaluate the impact of different advertisement strategies (ads vs. PSAs) on user conversions. By leveraging statistical tests and data visualization, we identify actionable insights for optimizing marketing campaigns.

---

## **Dataset**
The dataset is sourced from [Kaggle's Marketing A/B Testing Dataset](https://www.kaggle.com/datasets/faviovaz/marketing-ab-testing/data). It includes the following key columns:
- **Index**: Row index.
- **user_id**: Unique user identifier.
- **test_group**: Indicates whether a user saw an advertisement (`ad`) or a public service announcement (`psa`).
- **converted**: Boolean flag indicating whether the user converted (`True`) or not (`False`).
- **total_ads**: Total number of ads seen by the user.
- **most_ads_day**: Day of the week the user saw the most ads.
- **most_ads_hour**: Hour of the day the user saw the most ads.

---

## **Goals**
1. Determine the effectiveness of advertisements compared to PSAs in driving user conversions.
2. Understand user engagement patterns (day and hour of peak activity).
3. Provide data-driven recommendations for optimizing marketing strategies.

---

## **Analytical Approach**
1. **Descriptive Statistics**:
   - Summarize key metrics (e.g., conversion rates, ad exposure patterns).
   - Identify trends in user behavior.
2. **Statistical Testing**:
   - Use Chi-Square tests to examine relationships between categorical variables (e.g., test group and conversion status).
   - Employ non-parametric tests (Mann-Whitney U) for continuous variables like `total_ads`.
   - Conduct A/B testing (two-proportion z-test) to evaluate the difference in conversion rates.
3. **Visualization**:
   - Generate bar charts, histograms, and time-of-day analyses to support findings.
4. **Data-Driven Recommendations**:
   - Provide actionable insights for marketing teams based on statistical results.

---

## **Key Findings**
- **Ad Effectiveness**:
  - Ads have a higher conversion rate (**2.55%**) compared to PSAs (**1.79%**).
- **User Activity**:
  - Peak engagement occurs between **10:00–15:00**, with Friday being the most active day.
- **Ad Exposure**:
  - Most users see between **20–30 ads**, but outliers show extreme exposure (up to 2,065 ads), risking ad fatigue.
- **Conversion Patterns**:
  - Conversion rates are consistent across days, with Monday showing the highest rate (**3.28%**).

---

## **Technologies Used**
- **Programming Language**: Python
- **Libraries**: 
  - Pandas, NumPy (data manipulation)
  - Matplotlib, Seaborn (visualization)
  - Scipy, Statsmodels (statistical testing)

