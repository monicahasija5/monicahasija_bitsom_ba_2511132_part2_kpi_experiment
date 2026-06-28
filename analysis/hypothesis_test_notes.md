# Hypothesis Test Notes

## Metric Being Tested

The primary metric selected for hypothesis testing is **Paid Conversion Rate** because it is the North Star Metric for this experiment. The main objective of the new onboarding campaign is to increase the percentage of users who convert to a paid subscription.

---

## Null Hypothesis (H₀)

The Paid Conversion Rate of the Treatment group is equal to the Paid Conversion Rate of the Control group.

**H₀: pTreatment = pControl**

---

## Alternative Hypothesis (H₁)

The Paid Conversion Rate of the Treatment group is higher than the Paid Conversion Rate of the Control group.

**H₁: pTreatment > pControl**

---

## Type of Test

A **one-tailed (right-tailed) Two-Sample t-Test Assuming Unequal Variances** is used because the business objective is to determine whether the new onboarding campaign improves the Paid Conversion Rate.

---

## Significance Level

The significance level used for this analysis is:

**α = 0.05 (5%)**

---

## Reason for Choosing this Metric

Paid Conversion Rate is the most important success metric because it directly measures how effectively the onboarding campaign converts users into paying customers. An increase in this metric contributes directly to business growth and recurring subscription revenue.

---

## Decision Rule

- If the p-value is less than 0.05, reject the null hypothesis and conclude that the Treatment group has a significantly higher Paid Conversion Rate.
- If the p-value is greater than or equal to 0.05, fail to reject the null hypothesis because there is not enough statistical evidence to conclude that the Treatment group performed better.

---

## Business Interpretation

The hypothesis test will help determine whether the improvement in Paid Conversion Rate is statistically significant or simply due to random variation. The result of this test will support the final recommendation on whether the new onboarding experience should be launched to all users.