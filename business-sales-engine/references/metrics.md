# Commercial metrics: definitions before benchmarks

Fill [dashboard](../templates/metrics-dashboard.md). David Skok's SaaS metrics guide is a historical reference, not an October 2026 benchmark study [S14](sources.md). Formulas and controls below are operational definitions to adapt consistently.

| Metric | Definition | Main trap |
|---|---|---|
| Stage conversion | Eligible entrants reaching next stage / entrants, within a stated window | Mixing cohorts, stage changes, incomplete windows |
| Win rate | Wins / concluded opportunities (wins + losses), state exclusions | Removing no-decision losses |
| CAC | Fully scoped acquisition spend / acquired customers in matched cohort/window | Excluding sales labor or ignoring lag |
| CAC payback | CAC / monthly gross profit or contribution per acquired account | Using revenue; ignoring variable support |
| Logo churn | Lost starting customers / starting customers, period stated | Adding new customers to denominator |
| GRR | (Starting recurring revenue − churn − contraction) / starting revenue | Counting expansion or new revenue |
| NRR | (Starting revenue − churn − contraction + expansion) / starting revenue | Counting new accounts or masking logo churn |
| Cohort retention | Remaining original accounts / original accounts at cohort age | Comparing different ages |
| LTV | Expected discounted contribution/gross profit over customer life, definition stated | Extrapolating young cohorts forever |

For stable homogeneous subscriptions without expansion, a rough LTV = monthly ARPA × gross-margin fraction / monthly logo churn. It assumes stationary churn/margins, ignores discounting and is unreliable with zero churn, negative revenue churn, short histories or changing cohorts. Prefer bounded cohort cash-flow scenarios and avoid presenting the shortcut as measured LTV.

LTV/CAC ≥3 is a commonly used heuristic, not a universal gate. Check cost definitions, uncertainty, payback, financing and segment first. A high ratio from imagined long lifetimes is not permission to scale. Thresholds should be chosen from actual runway, contribution and risk tolerance.

Show new MRR, expansion, contraction and churn separately. Break out cash versus recognized/contracted revenue. Guardrail growth with capacity, quality, opt-outs and complaints. Use owner/source/update cadence for each metric; no denominator means no defensible rate. The [examples](../examples/unit-economics.md) show cross-checks and assumptions.
