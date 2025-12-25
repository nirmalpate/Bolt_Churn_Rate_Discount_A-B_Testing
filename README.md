# Bolt_Churn_Rate_Discount_A-B_Testing

This README is designed to reflect the technical depth and business acumen expected of a **Senior Growth Analyst at Bolt**. It structures your analysis into a professional "Executive Summary" that highlights both statistical rigor and marketplace strategy.

---

# Bolt Growth Experiment: Discounting Strategy Analysis

## 1. Executive Summary

This report evaluates the impact of a **€5 discount** targeted at churned riders. While the experiment aimed to drive revenue growth (ARPU), our analysis incorporates statistical significance, economic profitability, and long-term marketplace health (Guardrail Metrics).

**Final Recommendation:** **[DO NOT LAUNCH / LAUNCH]**

* *Based on: Statistical Power, Contribution Margin, and Repeat Purchase Rate.*

---

## 2. Hypothesis Framework

* **Primary Objective:** Increase Average Revenue Per User (ARPU) among the churned segment.
* **Null Hypothesis ():** The €5 discount has no significant effect on ARPU or Conversion.
* **Alternative Hypothesis ():** The €5 discount increases ARPU by at least 10% (MDE).
* **Success Metric:** Average Revenue Per User (ARPU).
* **Guardrail Metrics:** 1. **Contribution Margin:** (Revenue - Discount Cost) per user.
2. **Repeat Purchase Rate:** 30-day organic retention to monitor "Discount Addiction."

---

## 3. Methodology & Statistical Rigor

### Sample Size Calculation

Before analysis, we determined the required sample size to ensure a power of 80% and a confidence level of 95%:

* **Baseline ARPU ():** €10.00
* **Variance ():** 20
* **MDE:** 10% ()
* **Required :** **314 users per group** (628 total).

### Statistical Tests Applied

* **Independent T-Test:** Used for **Revenue (Continuous)** to compare means between Control and Treatment.
* **Chi-Square Test ():** Used for **Conversion and Retention (Categorical)** to analyze the frequency of "success" vs "failure."

---

## 4. Technical Implementation (Python)

The analysis was performed using `scipy.stats` and `pandas`. Key steps included:

1. **Data Cleaning:** Clipping outliers and handling null values.
2. **SRM Check:** Verified that the sample ratio between Control and Treatment was exactly 50/50 using a Chi-Square goodness-of-fit test.
3. **Inference:** Running the T-test and Chi-Square to extract p-values.

---

## 5. Economic & Risk Assessment

### Profitability Analysis

Statistical significance does not equal profitability. We calculated the **Incremental Profit**:

* **Incremental Revenue:** 
* **Total Cost:** 
* **ROI:** 

### Long-Term Risk (The "Leaky Bucket")

We evaluated the risk of **Cannibalization** and **Discount Sensitivity**. If the Treatment group shows a significant lift in short-term revenue but a decrease in **Repeat Purchase Rate**, the strategy is deemed unsustainable as it trains users to only book rides when subsidized.

---

## 6. Findings & Conclusion

* **Statistical Significance:** [e.g., ] — The result is statistically significant.
* **Economic Viability:** [e.g., ROI = -12%] — Despite the lift, the discount cost exceeds incremental gains.
* **Guardrail Status:** [e.g., Retention dropped by 2%] — High risk of long-term churn.

**Final Decision:** **No Launch.** The experiment is a "Fake Win"—positive revenue lift is offset by negative margins and a decay in long-term organic retention.

---

 

 
