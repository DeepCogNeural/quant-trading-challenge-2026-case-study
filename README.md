# Akuna Quant Trading Challenge 2026

This repository is a non confidential portfolio summary of my work in the 2026 Akuna Quant Trading Challenge. It contains no challenge prompt, submission code, platform export, private identifiers, or internal logs. It is not affiliated with or endorsed by Akuna Capital.

## Results

| Metric | Result |
| --- | --- |
| Overall evaluation | **19.70 of 20** points |
| Strategy score | **15.70 of 16** scored strategy cases |
| Evaluation cases | **20 of 20 passed** |
| Bankruptcies | **0** |
| Official final ranking | **Not yet announced** as of August 30, 2026 |

The 19.70/20 overall evaluation and 15.70/16 strategy score use different scoring denominators. The strategy score covers the 16 scored strategy cases in the captured platform evaluation; the other four cases were validation checks. Neither score is a public competition ranking, an award, real money trading performance, or a recruiting outcome.

## The problem

The challenge required a market maker for binary event contracts. The strategy had to estimate payout probabilities, quote prices and quantities under uncertainty, manage inventory, and remain within capital constraints while competing for simulated order flow.

## My approach

I built the strategy in Python around three connected components:

1. **Probability models:** a smoothed discrete transition model for rate movements and conditional Gaussian models of company log returns, fitted with ordinary least squares and adjusted for cross company residual covariance.
2. **Uncertainty aware pricing:** model derived probability bounds for rate, company value, and relative value contracts.
3. **Risk controlled execution:** dynamic whole cent quotes, adaptive quantities, inventory reduction logic, and maximum loss capital controls.

## Resume summary

> Built a Python market maker for rate, company valuation, and relative value binary options, combining smoothed discrete rate transitions, conditional Gaussian log return models, residual covariance, model derived uncertainty bounds, and inventory and capital constrained dynamic quoting; earned 19.70 of 20 overall evaluation points, passed all 20 cases, and recorded zero bankruptcies.

## Public scope

This page intentionally omits the challenge statement, source code, exact parameters and thresholds, order data, counterparty identifiers, competitor information, screenshots, run identifiers, hashes, and submission workflow.

## Updates

Official, attributable competition results will be added here if and when they are published.

* **August 30, 2026:** Official final ranking had not been announced.
