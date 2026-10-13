# Business Sales Engine 2.0

**English v2.0** · [Português v1](#português-v1) · [Español v1](#español-v1)

![Commercial Engine](assets/commercial-engine-overview.png)

A practical skill for diagnosing and building the commercial side of services, SaaS/PLG, B2B enterprise, digital/physical products and local businesses. It connects offer, pricing, acquisition, buying decisions, delivery, retention and proof through evidence-backed decisions and usable templates.

**The English edition is v2.0.0, reviewed 2026-10-13. Portuguese and Spanish retain v1 and are not content-equivalent to v2.** The repository's original artwork is conceptual; the maintained instructions and modules govern behavior.

| Language | Installable folder | Version |
|---|---|---|
| English (primary) | [business-sales-engine/](business-sales-engine/SKILL.md) | 2.0.0 |
| Português | [motor-comercial-negocios/](motor-comercial-negocios/SKILL.md) | v1 retained |
| Español | [motor-comercial-negocios-es/](motor-comercial-negocios-es/SKILL.md) | v1 retained |

## What changed

The single-file rule list is now an orchestrator with three modes: focused review, bottleneck diagnosis and complete-engine design. The skill loads only relevant references and completes practical templates rather than forcing thirteen deliverables into every request.

- Structured SPIN/gap discovery and MEDDPICC qualification.
- Buying committees, champion evidence, JOLT-style indecision diagnosis and conditional negotiation.
- Signal-based outbound with source verification, sender readiness and refusal/opt-out handling.
- Offer/pricing choices, contribution versus markup, capacity, CAC/payback and cohort retention/GRR/NRR.
- SaaS/PLG/PQL, founder sales, narrative, first useful result and delivery handoff.
- Honest proof/limits, bounded guarantees, referrals and decision-support content.
- AI-assisted research/call analysis with validation, plus dated assistant-brand audits.

Removed universal price multipliers, compulsory premium tiers, automatic guarantee stacking and fixed buyer-readiness percentages. Corrected the premium-mix example to **1.9× revenue** under explicit assumptions. LTV/CAC ≥3 remains a contextual heuristic, not a universal scaling gate.

## Package map

```text
business-sales-engine/
├── SKILL.md                  # orchestrator, decision tree, areas 0–11
├── trends.md                 # dated watchlist and semiannual review procedure
├── CHANGELOG.md
├── LICENSE
├── references/               # diagnosis, discovery, sales, economics, AI and sources
├── templates/                # 19 fillable operating tools
├── objections/library.md     # 15 diagnostic patterns: bad, good, evidence, stop
├── checklists/               # deal, call, proof/risk and agreement handoff
└── examples/                 # six labeled synthetic examples
```

Start with the [decision tree](business-sales-engine/SKILL.md). Study through [reading by section](business-sales-engine/references/reading-by-section.md); inspect [sources and limits](business-sales-engine/references/sources.md), [numerical examples](business-sales-engine/examples/unit-economics.md), [trends](business-sales-engine/trends.md) and [changelog](business-sales-engine/CHANGELOG.md).

## Installation

Clone the repository and copy **the entire language folder**, including supporting resources. Copying only `SKILL.md` breaks the v2 routing.

```bash
git clone https://github.com/C48H74/business-sales-engine.git
# Claude Code
mkdir -p ~/.claude/skills
cp -r business-sales-engine/business-sales-engine ~/.claude/skills/
# Codex
mkdir -p ~/.codex/skills
cp -r business-sales-engine/business-sales-engine ~/.codex/skills/
```

For a platform supporting skill-folder uploads, zip the English folder with all resources and import through that platform's supported skill flow. Folder layouts and installation interfaces can vary; consult the platform's current documentation.

## Usage

> Use business-sales-engine to review this offer and price. Keep this a focused review and identify unsupported claims.

> Use business-sales-engine to diagnose our SaaS funnel and churn from this cohort data. Compare explanations before recommending more acquisition.

> Use business-sales-engine to prepare enterprise discovery, a committee map and negotiation options. Mark unknowns rather than inventing buyer facts.

The skill content is English; responses follow the user's requested language. This does not mean the PT/ES source files have been translated to v2. Fillable fields are intentional; examples are simulations, not evidence of real clients or outcomes.

## Twelve maintained areas

| Step | Topic |
|---|---|
| 0 | Context, baseline and bottleneck hypotheses |
| 1 | Customer/problem plus structured discovery and qualification |
| 2 | Offer, dependencies and tested value levers |
| 3 | Price, billing models, economics and optional packages |
| 4 | Risk reduction and financially bounded commitments |
| 5 | Verified limits and buyer-relevant timing |
| 6 | Pipeline, committee, objections, indecision and negotiation |
| 7 | Commercial agreement preparation |
| 8 | Consent-based referrals after useful value |
| 9 | Measured proof, attribution and approved case studies |
| 10 | Website/content and validated AI assistance |
| 11 | Customer selection, delivery, retention and experiments |

![Commercial Engine Roadmap](assets/commercial-engine-roadmap.png)

![Trust and Evidence Loop](assets/trust-evidence-loop.png)

## Maintenance and attribution

Reviewed **2026-10-13**; next scheduled review **2027-04-13**. This is a documented reminder, not an installed automation. Provider rules should be rechecked before actual execution. Book/framework references identify provenance and study routes; no full-book reading or universal sales-performance validation is claimed.

V2 is an original paraphrased synthesis and adaptation. The source register credits framework originators and preserves the v1 influences: Alex Hormozi, Russell Raath, Jonathan Stark, Harrison Baron, John Jantsch, Joel Klettke, Andy Crestodina and ADALID Abogados. No copied book chapters or transcripts.

Educational commercial guidance. Specific legal, tax/accounting and regulated decisions require appropriate qualified review. Using a skill does not itself authorize sending messages, publishing customer information or accepting agreements.

## Português v1

Versão original mantida em [motor-comercial-negocios/](motor-comercial-negocios/SKILL.md). Não contém os módulos e templates da v2 inglesa. Instalação: `cp -r business-sales-engine/motor-comercial-negocios ~/.claude/skills/`.

## Español v1

Versión original conservada en [motor-comercial-negocios-es/](motor-comercial-negocios-es/SKILL.md). No contiene los módulos y las plantillas de la v2 inglesa. Instalación: `cp -r business-sales-engine/motor-comercial-negocios-es ~/.claude/skills/`.

## License and author

[CC BY 4.0](LICENSE) — use, adapt and redistribute, including commercially, with attribution and an indication of changes.

Daniel de Souza Paixão — [LinkedIn](https://www.linkedin.com/in/daniel-paixao-b5988230).
