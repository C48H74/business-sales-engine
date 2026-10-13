# AI in the sales process

Load when the user wants to apply AI to prospecting, calls, forecasting, timing or content. Principle: AI raises the floor of mediocre work and the bar for what counts as personal; it does not replace judgment or relationships.

## Where it helps, with guardrails

| Use | How | Guardrail |
|---|---|---|
| **Account research** | Summarize public info, recent news, hiring, product changes into a one-paragraph brief with sources | Verify one fact before using it in a message; hallucinated details end conversations |
| **Personalization at scale** | Draft first lines from real signals; you edit | Since everyone does this, generic "AI-personalized" lines read as template. The bar is a specific, true, recent observation |
| **Call transcription and analysis** | Score against `checklists/post-call-rubric.md`: talk ratio, question count and types, next step captured, objections raised, MEDDPICC gaps | Review the scoring on a sample; models over-credit polite calls |
| **Objection mining** | Cluster objections from transcripts and emails; update `objections/library.md` | Keep the buyer's wording |
| **Proposal and business-case drafts** | Fill `templates/business-case-onepager.md` from discovery notes | Numbers come from the client, never generated |
| **Pipeline hygiene** | Flag deals with no next step, stale stages, single threads | Rules-based first; it's cheaper and more reliable |
| **Forecasting and timing ("who will buy, when")** | Intent/propensity scores from signals | See calibration note below |
| **Brand presence in assistants** | Ask several AI assistants how they describe your company, category and alternatives; fix with factual pages | Re-check quarterly; answers change |
| **Role-play** | Rehearse discovery and objections with a model playing the buyer persona | Treat as practice, not as research |

## Calibration note on predictive scores

Models that predict human decisions (who will buy, when a deal closes, which lead will convert) are much weaker than vendors claim, as Narayanan and Kapoor argue in *AI Snake Oil*: outcomes depend on information the model never sees. Before trusting a propensity score:
1. Compare it against a simple baseline (recency of signal + fit) on your own closed deals.
2. Check calibration: of leads scored 80%, did roughly 80% convert?
3. Use scores to **prioritize** work, never to **skip** discovery or to decline a lead automatically.

## What not to automate

- Discovery conversations (the buyer notices).
- Negotiation.
- The referral ask.
- Any message that implies a human relationship that doesn't exist.

## Data and disclosure

- Record calls only with consent per local law; say so at the start.
- Keep client data out of tools that train on inputs unless contractually covered.
- Don't let a model invent references, logos or results. Every claim traces to `references/delivery-retention.md` proof rules.

## A workable setup for a small team

1. Research brief per account (AI draft, 2-minute human check).
2. Sequence drafts from `templates/5-touch-sequence.md` with signal-based first lines (human edits).
3. Call transcripts scored weekly against the rubric; one coaching note per rep.
4. Monthly objection mining into the library.
5. Quarterly brand-in-assistants check.
