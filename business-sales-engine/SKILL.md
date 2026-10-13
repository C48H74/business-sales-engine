---
name: business-sales-engine
description: "Design, diagnose or run the sales engine of any business: offer and pricing, lead qualification (MEDDPICC, gap selling), discovery calls (SPIN), objections and no-decision deals (JOLT), negotiation and discounts, buying committees and multithreading, outbound prospecting and email deliverability, pitch narrative, founder-led sales, PLG and product-qualified leads, B2B enterprise, SaaS, churn and retention, CAC/LTV/payback metrics, guarantees, scarcity, referrals, case studies and content. Triggers: sales, pricing, offer, deal stuck, 'I'll think about it', negotiation, cold email, cold call, discovery call, buying committee, churn, pipeline, proposal, business case."
metadata:
  version: "2.0.0"
  last_reviewed: "2026-10-13"
  review_cadence: "Every 6 months: re-check trends.md, metrics benchmarks and reading-list.md against new sources."
  license: "CC BY 4.0"
---

# Business Sales Engine (v2)

This file is an **orchestrator**, not an encyclopedia. It decides which module to load for the situation at hand. Theory lives in `references/`, fillable artifacts in `templates/`, scripts in `objections/`, go/no-go gates in `checklists/`, worked contrasts in `examples/`. Load only what the situation needs.

Reply in the user's language. Be direct. Every recommendation must end in an artifact, a script or a number, never in a slogan.

## Step 0 — Pick the mode

| Mode | When | Deliverable |
|---|---|---|
| **Quick review** | User brings one thing (an email, a price, a proposal, an objection) | Verdict + corrected version + one reason per change |
| **Bottleneck diagnosis** | "I need more clients / revenue / margin" with no clear cause | Diagnosis across the 5 checkpoints below + the single next experiment (use `templates/experiment-card.md`) |
| **Full build** | New offer, new segment, new motion, or a founder starting to sell | The relevant subset of the 12-step map, each step closed with its template |

Never default to the full build. Ask which mode if unclear; if the user is absent, pick the smallest mode that answers the request and say so.

## Step 1 — Decision tree: what to load

| Situation | Load |
|---|---|
| "I need more clients" / unclear bottleneck | **Diagnosis sequence** below, then `references/metrics.md` |
| Offer is vague, price was guessed, tiers are a mess | `references/offer-pricing.md` + `templates/pricing-tier-worksheet.md` |
| Build pipeline / prospect / cold outreach | `references/outbound.md` + `templates/5-touch-sequence.md` + `templates/cold-call-scripts.md` + `examples/cold-email-good-vs-bad.md` |
| First call with a prospect | `references/discovery.md` + `templates/discovery-call-guide.md` + `examples/discovery-call-transcript.md` |
| Qualify an enterprise / large deal | `references/qualification.md` + `templates/meddpicc-scorecard.md` |
| Deal stalled, "I'll think about it", no next step | `references/jolt.md` + `objections/library.md` |
| Any objection, price pushback | `references/objections.md` + `objections/library.md`; for price also `references/negotiation.md` |
| Discount request, procurement, contract terms | `references/negotiation.md` + `templates/business-case-onepager.md` |
| Only one contact in the account | `references/multithreading.md` + `templates/buying-committee-map.md` |
| Pitch, demo, deck, website hero | `references/narrative.md` + `templates/pitch-narrative.md` |
| Founder selling for the first time, hiring first rep | `references/founder-sales.md` |
| Self-serve product with usage signals | `references/plg-pql.md` |
| Guarantee, refund policy, urgency, scarcity | `references/guarantees-scarcity.md` |
| Churn, onboarding, scope creep, referrals, case studies | `references/delivery-retention.md` |
| Website, content, what to publish | `references/content.md` |
| Using AI for prospecting, call analysis, timing | `references/ai-in-sales.md` |
| Persuasion mechanics, exact phrases | `references/psychology.md` |
| Before a forecast or pipeline review | `checklists/deal-review.md` |
| After any sales call | `checklists/post-call-rubric.md` |
| "Is this still current?" | `trends.md` |
| "What should I read to go deeper?" | `reading-list.md` |

## Step 2 — Diagnosis sequence (before concluding anything)

"I need more marketing" is a hypothesis, not a diagnosis. Check in this order and stop at the first broken link:

1. **Reach** — Are enough of the right people seeing the offer? (impressions, list size, meetings booked)
2. **Lead quality** — Of those who respond, how many fit the ideal profile? (qualified / total)
3. **Conversion** — Of qualified leads, how many buy, and where do they drop? (stage-by-stage, see `references/qualification.md` stage gates)
4. **Capacity** — Can the business deliver more without quality collapsing? (utilization, backlog)
5. **Retention and expansion** — Do customers stay and buy more? (churn, NRR, referrals)

Fixing reach when conversion is broken buys more losses. Fixing conversion when capacity is full buys angry customers. Numbers for each checkpoint: `references/metrics.md`.

## Step 3 — Core principles (revised in v2)

1. **A business is arbitrage with a margin of safety.** Revenue per customer must exceed the cost to acquire and serve them with room for error. Measure it: CAC, payback, contribution margin, retention by cohort.
2. **Order of work: Offer → Price → Sales → Demand**, but diagnose first (Step 2). More demand on a weak offer exposes the weakness faster.
3. **Trust is the asset.** The buyer carries money, time and reputational risk. Every artifact should lower that risk with evidence, not adjectives.
4. **Positioning follows demand, cost and capacity**, not a slogan. Premium, mid-market and volume all work when the unit economics close. The "death zone" is any position where price, cost to serve and buyer expectations don't match each other.
5. **Sell outcomes the buyer defined**, not features you built. Discover what they value before assuming speed, price or convenience is the lever.
6. **Supply and demand set the price ceiling; cost sets the floor; alternatives set the reference.** When demand exceeds capacity, raise price or cut slots; when it doesn't, fix the offer before cutting price.
7. **No decision is the main competitor.** Indecision loses more qualified deals than rivals do; treat it as an objection with its own playbook (`references/jolt.md`).
8. **The market exposes vagueness.** A vague offer shows up as unqualified leads; illogical pricing shows up in negotiation; the wrong customer shows up in delivery; empty content shows up as silence.

## Step 4 — The 12-step map (what a full build covers)

| # | Step | Module | Closes with |
|---|---|---|---|
| 0 | Context intake | below | Filled intake |
| 1 | Ideal customer, pain, research | `references/discovery.md` (Mom Test section) | Customer research notes |
| 2 | Offer | `references/offer-pricing.md` | Offer statement |
| 3 | Economics and pricing | `references/offer-pricing.md`, `references/metrics.md` | `templates/pricing-tier-worksheet.md` |
| 4 | Qualification and discovery | `references/qualification.md`, `references/discovery.md` | `templates/meddpicc-scorecard.md`, `templates/discovery-call-guide.md` |
| 5 | Narrative and proof | `references/narrative.md`, `references/delivery-retention.md` | `templates/pitch-narrative.md` |
| 6 | Risk reduction, scarcity | `references/guarantees-scarcity.md` | Guarantee with exposure math |
| 7 | Pipeline and outbound | `references/outbound.md` | `templates/5-touch-sequence.md` |
| 8 | Objections, indecision, negotiation | `references/objections.md`, `references/jolt.md`, `references/negotiation.md` | `templates/business-case-onepager.md` |
| 9 | Buying committee | `references/multithreading.md` | `templates/buying-committee-map.md` |
| 10 | Contract and handoff | `references/delivery-retention.md` (contract section) | Contract checklist, handoff doc |
| 11 | Delivery, retention, referrals, case studies | `references/delivery-retention.md` | 30/60/90 plan, referral moment, case study consent |
| 12 | Content and AI leverage | `references/content.md`, `references/ai-in-sales.md` | Content plan, AI workflow |

Cross-cutting: `references/metrics.md` (measure every step), `references/psychology.md` (phrasing), `templates/experiment-card.md` (change one thing at a time).

## Context intake (ask only what is missing)

1. What is sold, to whom, who signs, who uses.
2. Market and country (contract norms, procurement habits).
3. Price today, real cost to deliver, hours per customer.
4. Capacity: customers per week/month, start cadence.
5. Where customers come from now; conversion by stage if known.
6. Proof available: results with numbers, testimonials, cases, certifications.
7. Deal size and cycle length (decides whether MEDDPICC and multithreading apply).
8. Goal and constraint: more customers, more margin, less effort, recurring revenue, faster decisions.

## Inviolable rules

1. Every call ends with a scheduled next step, or the deal is marked at risk.
2. No price goes out without a quantified pain or a business case (`templates/business-case-onepager.md`).
3. Discounts are traded, never given: "I can do X if you can do Y."
4. Enterprise deals are never single-threaded.
5. Treat "no decision" before treating the competition.
6. Scarcity and deadlines are real or absent. Invented urgency is a trust withdrawal you cannot repay.
7. Proof is documented and authorized. Label simulations as simulations.
8. One variable per experiment, with a stop rule.

## Funnel stage gates (objective criteria to advance)

| Stage | Exit criterion |
|---|---|
| Lead | Fits profile on 2 of 3: segment, role, trigger signal |
| Qualified | Pain stated in their words + quantified impact + a named decision process |
| Discovery done | MEDDPICC scorecard with no red on Pain, Champion, Decision Process |
| Proposal | Business case accepted by champion; economic buyer identified and reached |
| Negotiation | Written criteria met; paper process (legal, security, procurement) mapped with dates |
| Closed | Signed + kickoff scheduled + handoff doc sent |

## Output contracts

**Quick review:** 1) verdict in one line; 2) the corrected artifact; 3) a change log, one reason per change; 4) one thing to test next.

**Bottleneck diagnosis:** 1) the five checkpoints with the number or "unknown" for each; 2) the broken link; 3) one experiment card; 4) what to measure in 30 days.

**Full build:** the steps that apply from the 12-step map, each closed with its template, then a 30-day plan with owners and metrics. Never pad with steps that don't apply.

## What this skill refuses to do

- Use BANT as a gate (keep budget and timing as signals only).
- Write "hope you're well" or "I'd like to introduce our company" openers.
- Present features and benefits as a pitch structure.
- Recommend email volume without deliverability setup.
- Stack guarantees by default or promise outcomes outside the seller's control.
- Quote percentages without a source and a population ("97% aren't ready to buy" is retired).
- Give motivational lines in place of an action.

## Maintenance

See `CHANGELOG.md`. Trends and benchmarks age fastest: re-verify `trends.md` and the heuristics in `references/metrics.md` at each review date. Sources per section: `reading-list.md`.
