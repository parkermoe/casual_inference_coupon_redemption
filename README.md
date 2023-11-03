# Personalized Coupon Redemption Analysis

## Introduction

This project investigates the effectiveness of personalized coupon campaigns versus non-personalized ones. Using data from various sources, we examine whether personalization in coupon distribution leads to a significant increase in redemption rates.

## Hypothesis

We test the following hypotheses to understand the impact of personalized coupon campaigns:

### Null Hypothesis ($$H_0$$):
$$H_0: \mu_{\text{personalized}} = \mu_{\text{non-personalized}}$$
The null hypothesis states that there is no significant difference in the redemption rates between personalized and non-personalized coupons.

### Alternative Hypothesis ($$H_1$$):
$$H_1: \mu_{\text{personalized}} \neq \mu_{\text{non-personalized}}$$
The alternative hypothesis suggests that personalized coupon campaigns lead to a significantly different redemption rate compared to non-personalized campaigns.

## Datasets

The analysis utilizes four primary datasets:

1. **Campaign Table** (`campaign_table.csv`): Contains information about the coupons sent to households.
2. **Household Demographics** (`hh_demographic.csv`): Demographic information of the households.
3. **Coupon Details** (`coupon.csv`): Details of the coupons associated with campaigns.
4. **Coupon Redemption** (`coupon_redempt.csv`): Data on which coupons were redeemed by households.

## Methodology

The project follows these steps for analysis:

1. **Data Preprocessing:** Standardizing and cleaning data for analysis.
2. **Redemption Rate Calculation:** Determining the rate of coupon redemption for personalized and non-personalized campaigns.
3. **Treatment and Control Group Formation:** Creating comparable groups for analysis.
4. **Propensity Score Matching:** Matching households based on propensity scores to control for confounding variables.
5. **Statistical Analysis:** Performing statistical tests to compare the redemption rates of the matched groups.

## Findings

Our analysis did not find a statistically significant difference in redemption rates between personalized and non-personalized coupon campaigns. The Mann-Whitney U test yielded a p-value of 0.3173, leading us to fail to reject the null hypothesis.

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

