# A/B Testing: Landing Page Conversion & Engagement Analysis

## Project Overview
A streaming platform conducted an A/B test to evaluate whether a new simplified landing page improves user engagement and subscription conversions.

The analysis compares:
- Conversion rate (subscription sign-ups)
- User session time (engagement)

Statistical hypothesis testing is used to support data-driven product decisions.

---
## Dataset
The dataset contains user-level interaction data from a streaming platform experiment.  
All users are from Nigeria.

Key variables include:
- `group`: A (Control) or B (Variant)
- `converted`: 1 if the user subscribed, 0 otherwise
- `session_time`: Time spent on the landing page (minutes)
- `device`, `traffic_source`, `pages_visited`, `previous_visits`

---

## Methodology

### Data Cleaning
- Removed rows with missing values for required metrics
- Removed duplicate records
- Verified and confirmed correct data types

### Metrics
- **Primary metric:** Conversion rate
- **Secondary metric:** Session time

### Statistical Tests
- **Z-test (proportion test)** to compare conversion rates
- **Independent two-sample t-test** to compare mean session time

---

## Results

### Conversion Rate (Z-test)
- Z-statistic: **4.26**
- p-value: **0.00001**

The new landing page (Group B) has a significantly higher conversion rate than the control.

---

### Session Time (T-test)
- t-statistic: **12.47**
- p-value: **< 0.001**

Users exposed to the new landing page spent significantly more time on the platform.

---

## Final Recommendation
The new simplified landing page (Group B) outperforms the current version in both conversion rate and user engagement.

**Recommendation:** The company should implement the new landing page.
