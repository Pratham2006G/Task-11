README – A/B Testing Analysis

Project: A/B Test Analysis on Advertisement vs PSA Group

Objective:
The goal of this analysis is to determine whether advertisements (Ad group) result in a higher conversion rate compared to public service announcements (PSA group).

Dataset:
The dataset contains 6 columns:
- user_id
- Test group (Ad / PSA)
- Converted (0 / 1)
- Total ads
- Most ads day
- Most ads hour

Only 'Test group' and 'Converted' columns were used for the A/B test analysis. Other columns were ignored.

Steps Performed:
1. Data Loading: The dataset was loaded into Google Colab.
2. Data Exploration: Columns and unique values were checked.
3. Group Segmentation: Users were divided into Control (PSA) and Test (Ad) groups.
4. Conversion Rate Calculation: Average conversion for each group was calculated.
5. Hypothesis Formulation:
   - Null Hypothesis (H0): No difference in conversion rates.
   - Alternative Hypothesis (H1): Significant difference exists.
6. Statistical Testing: Chi-square test was applied to check significance.
7. Decision Making: Based on p-value (0.00259) and alpha (0.05), null hypothesis was rejected.
8. Visualization: Bar chart plotted to compare conversion rates.
9. Summary Files Generated:
   - ab_test_summary.csv : Contains conversion rates, p-value, and decision.
   - ab_test_findings.txt : Contains detailed analysis and interpretation.
   - final_recommendation.txt : Contains actionable business recommendation.

Results:
- Control (PSA) Conversion Rate: 0.03058
- Test (Ad) Conversion Rate: 0.04929
- P-Value: 0.00259
- Decision: Reject Null Hypothesis
- Conclusion: Ads significantly increase conversions compared to PSA.

Files Included: ab_test_summary.csv final_recommendation.txt
Task notebook: task11_abtest.ipynb

Notes:
- Analysis was conducted entirely in Google Colab.
- Only necessary columns (Test group, Converted) were used.
- This project demonstrates A/B testing, hypothesis testing, and interpretation for business decisions.
