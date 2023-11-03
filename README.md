# Personalized Coupon Redemption Analysis

## Introduction

This project investigates the effectiveness of personalized coupon campaigns versus non-personalized ones. Using data from various sources, we examine whether personalization in coupon distribution leads to a significant increase in redemption rates.

## Hypothesis

We test the following hypotheses to understand the impact of personalized coupon campaigns:

### Null Hypothesis: 

$$H_0: \mu_{\text{personalized}} = \mu_{\text{non-personalized}}$$
The null hypothesis states that there is no significant difference in the redemption rates between personalized and non-personalized coupons.

### Alternative Hypothesis:
$$H_1: \mu_{\text{personalized}} \neq \mu_{\text{non-personalized}}$$
The alternative hypothesis suggests that personalized coupon campaigns lead to a significantly different redemption rate compared to non-personalized campaigns.

## Datasets

The analysis utilizes four primary datasets:

1. **Campaign Table** (`campaign_table.csv`): Contains information about the coupons sent to households.
2. **Household Demographics** (`hh_demographic.csv`): Demographic information of the households.
3. **Coupon Details** (`coupon.csv`): Details of the coupons associated with campaigns.
4. **Coupon Redemption** (`coupon_redempt.csv`): Data on which coupons were redeemed by households.

The dataset along with a detailed description can be found here: [Data Description](https://github.com/Lanbig/CSC465-visualization-project/blob/master/Dataset/dunnhumby%20-%20The%20Complete%20Journey%20User%20Guide.pdf)

## Methodology

The project follows these steps for analysis:

1. **Data Preprocessing:** Standardizing and cleaning data for analysis.
2. **Redemption Rate Calculation:** Determining the rate of coupon redemption for personalized and non-personalized campaigns.
3. **Treatment and Control Group Formation:** Creating comparable groups for analysis.
4. **Propensity Score Matching:** Matching households based on propensity scores to control for confounding variables.
5. **Statistical Analysis:** Performing statistical tests to compare the redemption rates of the matched groups.


## Findings

Upon analysis, the observed average redemption rate for households that received personalized coupons (Type A) was approximately \( 0.0833 \), or \( 8.33\% \). In contrast, the observed rate for households that were not targeted with personalized coupons (Type B and C) was roughly \( 0.0146 \), or \( 1.46\% \).

This observational data initially suggests a markedly higher effectiveness of personalized coupons in driving redemptions—a near \( 5.7 \)-fold increase over non-personalized ones, which would have significant implications for marketing strategies focused on personalization.

However, when these results were subjected to a rigorous statistical analysis using matched samples to control for confounding variables, the evidence did not support a statistically significant difference between the two groups. The Mann-Whitney U test returned a p-value of \( 0.3173 \), compelling us to maintain the null hypothesis.

This finding brings to light the importance of statistical testing in validating business strategies. While personalized marketing may intuitively seem advantageous, the lack of statistical significance in this case indicates that such an approach did not demonstrably enhance coupon redemption rates within the scope of our study.

For businesses, this underscores the need to critically evaluate the impact of personalized marketing campaigns. It may prompt a re-examination of personalization techniques or a deeper investigation into other potential influences on coupon use. In the face of these results, businesses are advised to consider a broader spectrum of marketing strategies and perhaps integrate additional customer engagement tactics to bolster the effectiveness of coupon campaigns.


## Replicating the Analysis

To replicate this analysis:

1. Clone the repository to your local machine.
2. Ensure you have `Python 3.x` and the required packages (`pandas`, `scipy`, `matplotlib`, `causalml`, `sklearn`) installed.
3. Run the Jupyter notebooks in order, following the instructions within each notebook.

## Conclusion

The statistical analysis suggests that personalized coupons do not significantly increase redemption rates over non-personalized coupons within our dataset. However, further research with different data, methodologies, or additional factors could yield different insights.

## Contact

For any queries or discussions regarding this analysis, please open an issue in this repository or contact me directly.

---

**Author:** Parker Moesta

