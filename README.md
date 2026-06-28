# KPI Experiment Analysis

## Business Context

This project analyzes an A/B experiment conducted for a subscription-based digital product company. The company introduced a new onboarding campaign and wanted to find out whether it performs better than the existing onboarding process.

The users were divided into two groups:

* **Control Group:** Existing onboarding experience
* **Treatment Group:** New onboarding experience

The main objective was to decide whether the new onboarding campaign should be launched to all users based on the experiment results.

---

## Dataset Description

The dataset contains user-level data collected during the A/B experiment. It includes information related to user activity, onboarding, paid conversion, engagement, revenue, refunds, and support tickets.

Before starting the analysis, the dataset was checked for data quality. The following checks were performed:

* Missing values
* Duplicate user IDs
* Group counts
* Invalid binary values
* Revenue outliers
* Region distribution across groups

After completing these checks, the dataset was used for KPI analysis and hypothesis testing.

---

## North Star Metric

The North Star Metric selected for this experiment is **Paid Conversion Rate**.

This metric was chosen because the main objective of the onboarding campaign is to increase the number of users who become paid subscribers.

---

## KPI Tree Summary

The KPI Tree was created using **Paid Conversion Rate** as the North Star Metric.

The main KPI drivers are:

* User Acquisition
* User Activation
* User Engagement

Guardrail metrics such as **Support Ticket Rate** and **Refund Rate** were also included to make sure that higher conversions did not negatively affect the user experience.

---

## Experiment Analysis Approach

The experiment was completed in the following steps:

1. Performed data quality checks.
2. Compared the Control and Treatment groups using summary metrics.
3. Analyzed important metrics across different user segments using Pivot Tables.
4. Performed a one-tailed hypothesis test.
5. Evaluated guardrail metrics.
6. Prepared the final business recommendation based on the analysis.

---

## Hypothesis Test Summary

A one-tailed Two-Sample t-Test Assuming Unequal Variances was performed using the Paid Conversion Rate.

The one-tailed p-value obtained from the test was **0.00053**, which is less than the significance level of **0.05**.

Based on this result, the null hypothesis was rejected. This shows that the Treatment group achieved a statistically significant improvement in Paid Conversion Rate.

---

## Guardrail Metrics Considered

The following guardrail metrics were reviewed before making the final recommendation:

* Support Ticket Rate
* Refund Rate
* Average Days to Convert

The analysis showed that users converted faster in the Treatment group. Refund Rate increased slightly but remained very low. Support Ticket Rate increased noticeably and should continue to be monitored after launch.

---

## Final Recommendation

Based on the analysis, the recommendation is to **launch the new onboarding campaign**.

The Treatment group showed better Paid Conversion Rate, higher Engagement Score, faster user conversion, and slightly better Average Revenue per User.

Although the Support Ticket Rate increased, the overall results support launching the new onboarding experience while monitoring customer support requests after deployment.

---

## Assumptions and Limitations

* The analysis is based only on the dataset provided for this experiment.
* User behaviour may change over a longer period of time.
* The recommendation is based on the available experiment results and selected business metrics.

---

## Screenshots Included

The repository contains the following screenshots:

* `summary_metrics.png`
* `hypothesis_test_output.png`
* `kpi_tree_preview.png`
