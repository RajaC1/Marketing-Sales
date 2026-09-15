---
name: ab-test-analyzer
description: Interpret A/B or multivariate test results (conversion rates, sample sizes) for marketing/sales experiments, check statistical validity, and recommend next steps. Use when the user pastes test results or asks whether a test win is real. Difficulty: Advanced.
---

# A/B Test Result Analyzer

## Inputs to gather
- Variant names, visitors/sends per variant, conversions per variant
- Test duration and what was changed between variants
- Primary metric being optimized (CTR, conversion rate, reply rate, etc.)

## Process
1. Compute conversion rate per variant from the raw numbers given — show the arithmetic, don't just assert a winner.
2. Estimate statistical significance using a two-proportion z-test approximation; state the resulting p-value or confidence level and the required sample size for the effect size seen, so the user can judge if the test ran long enough.
3. Flag common validity problems: sample size too small, test stopped early ("peeking"), seasonality/day-of-week skew, multiple metrics tested without correction.
4. If the result is not statistically significant, say so plainly rather than declaring a winner — recommend whether to keep running or redesign the test.
5. If significant, recommend the concrete next action (ship the winner, run a follow-up test on the next variable, roll out to 100%).

## Rules
- Do not overstate confidence from small samples (e.g., 12 vs 40 conversions is not a reliable winner even if the rate differs).
- Always show your calculation, not just a conclusion, so the user can verify it.
- If the user hasn't given both visitor counts and conversion counts, ask for them rather than estimating.
