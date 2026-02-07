# recommender_system-Teste-A/B

A/B Test Analysis — Recommender System
# Project Overview

This project presents a complete analysis of an A/B test conducted by an international e-commerce company. The objective of the experiment was to evaluate whether the implementation of an improved recommendation system could increase user conversion rates throughout the purchase funnel.

The analysis covers data preparation, exploratory analysis, funnel construction, statistical hypothesis testing, and business recommendations based on the results.

# Objective

The company introduced a new recommendation system and expected it to improve user engagement and conversions within 14 days after registration. Specifically, the experiment aimed for at least a 10% increase in the following funnel stages:

Product page views

Add-to-cart events

Purchases

The key business question was:

Should the new recommendation system be launched?

# Datasets Used

The analysis was based on four datasets:

ab_project_marketing_events_us.csv — Marketing campaign calendar

final_ab_new_users_upd_us.csv — Newly registered users

final_ab_events_upd_us.csv — User interaction events

final_ab_participants_upd_us.csv — Experiment participants and group assignments

# Methodology

The project followed a structured analytical workflow:

1. Data Preparation

Converted data types (especially date fields)

Checked for missing values and duplicates

Identified users enrolled in multiple experiments and removed them to prevent contamination

Filtered the dataset to include only participants from the recommender_system_test

2. Exploratory Data Analysis (EDA)

Validated the experiment structure

Evaluated participant distribution across groups

Confirmed inconsistencies such as:

Smaller sample size than planned

Uneven group split

Potential seasonality effects (holiday shopping period)

3. Funnel Construction

A conversion funnel was built using unique users at each stage:

Base → Product Page → Cart → Purchase

Conversion rates were calculated relative to the experiment population to ensure robust interpretation.

4. Hypothesis Testing

A one-tailed Z-test for proportions was applied to determine whether the treatment group (B) outperformed the control group (A).

Hypotheses:

H0: B ≤ A (the new system does not improve conversions)

H1: B > A (the new system improves conversions)

# Key Findings

The treatment group did not outperform the control group in any funnel stage.

All Z-test results failed to reject the null hypothesis.

Negative Z statistics suggest the treatment group may actually perform worse.

Additionally, the experiment did not reach the planned sample size, which may limit statistical power.

 # Experiment Limitations

Several factors should be considered when interpreting the results:

The final sample size (~2,800 users) was significantly below the planned 6,000 participants.

Groups were unevenly distributed.

The test occurred during the holiday season, a period associated with atypical purchasing behavior.

Some users may not have completed the full 14-day observation window.

Despite these limitations, the results were consistent across all funnel metrics.

Business Recommendation

The new recommendation system should NOT be launched at this time.

The experiment showed no statistically significant improvements and indicated potential performance decline compared to the control group.

# Recommended Next Steps:

Investigate why the treatment reduced product page engagement.

Review the recommendation algorithm and placement strategy.

Consider running a new experiment with:

Balanced group allocation

Larger sample size

A less seasonally biased testing window
