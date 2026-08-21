# A/B Testing: Landing Page Conversion Rate Experiment

Statistical significance analysis of a simulated A/B test (5,000 users per group) comparing a control landing page against a redesigned variant, using proper hypothesis testing rather than raw percentage comparison.

## Key Results
- **Control conversion rate:** 9.86% | **Variant conversion rate:** 11.18%
- **Absolute lift:** +1.32 pts | **Relative lift:** +13.4%
- **Two-proportion z-test:** z = 2.151, p = 0.0315 → statistically significant
- **Chi-square test (cross-check):** χ² = 4.488, p = 0.0341 → confirms significance
- **95% CI on lift:** [+0.12, +2.52] percentage points (excludes zero)

## Methodology
1. Simulate randomized controlled experiment data (Bernoulli conversion trials)
2. Compute descriptive conversion rates and lift
3. Two-proportion z-test for significance
4. Chi-square test of independence as a cross-check
5. 95% confidence interval on the lift

## Visualization
![A/B test results](ab_test_charts.png)

## Tools
Python, NumPy, pandas, SciPy, Matplotlib

## Files
- `ab_test_analysis.py` — full analysis script
- `ab_test_charts.png` — conversion rate + lift CI chart
