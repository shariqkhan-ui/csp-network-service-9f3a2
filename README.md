# CSP Network vs Service — analysis

Interactive report: https://shariqkhan-ui.github.io/csp-network-service-9f3a2/

## Summary
Active CSPs (userbase >=20) scored on three metrics over the last 90 days:
- **OOR%** — device out-of-reach rate (optical/PNM devices only; numeric TP-Link IDs excluded). Low = good network.
- **Service SLA%** — partner-reported service-ticket SLA (3-mo). High = good.
- **Complaint% (daily)** — genuine internet complaint tickets per day / active customers (auto "supply-down" excluded). Low = good.

CSPs split into Good- vs Bad-Network at the median OOR%. The Good-Network cohort's median SLA (80.0%) and daily complaint (0.284%) are the **benchmark**. Both cohorts are graded against it.

## Key insights
- Good- and Bad-Network CSPs **fail at almost the same rate**: 33.0% of good-network vs 32.4% of bad-network CSPs are worse than benchmark on both complaints and SLA.
- 27.9% of Bad-Network CSPs **beat the benchmark on both** — weak network, excellent service.
- Complaint rate tracks **Service SLA, not OOR**. Doubling OOR barely moves complaints.

## Actionables
1. Fix the 93 **Failing** bad-network CSPs with an ops/SLA intervention (not network upgrades).
2. Study the 80 **Resilient** bad-network CSPs and replicate their service playbook.
3. Coach the 64 **SLA-slow** CSPs before complaints rise.
4. Root-cause the 50 **Complaints-high** CSPs (tickets closed in time but complaints persist).
5. Stop treating "bad network" as the reason for poor service — good-network CSPs fail at the same rate.

`csp_metrics.csv` holds the full per-CSP numbers.
