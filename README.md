# 05 — Business Development

> Part of the **Kojiki Decision System**. This repo is the
> **Business Development** line. It references the shared ontology in
> [`00-kojiki-ontology`](https://github.com/robfuj/kojiki-ontology) for the
> canonical schemas, taxonomy, decision-rights, and handoff standards.

## Primary question
> What external relationships create strategic value?

## Purpose
Create and structure external relationships that expand capabilities, distribution, economics, or strategic position.

## Sub-functions
Partner Strategy, Partner Sourcing, Strategic Alliances, Channel Partnerships, Ecosystem Development, Partnership Operations, Relationship Management

## Typical roles
VP Business Development, VP Strategic Partnerships, BD Director, Partnerships Director, BD Manager, Strategic Alliances Manager

## Inputs
Partner capabilities, strategic objectives, incentives, economics, relationship context.

## Outputs
Partnership structures, alliances, channels, joint initiatives, partner performance.

## Learning focus
Partner fit; incentive alignment; negotiation outcomes; partner reliability; partnership failure signals.

## Operating tree
```text
STRATEGIC NEED →
 PARTNER UNIVERSE →
 TARGET →
 FIT →
 STAKEHOLDERS →
 MUTUAL VALUE →
 ALIGNMENT →
 STRUCTURE →
 NEGOTIATION →
 EXECUTION →
 PERFORMANCE →
 EXPANSION / RESTRUCTURE / EXIT
```

## Decision states
```text
IDENTIFIED → QUALIFIED → NEGOTIATING → LAUNCHED → PERFORMING → EXPANDING → RESTRUCTURING → EXITED
```

## Decision outputs
`Pursue · Validate · Negotiate · Launch · Expand · Restructure · Exit`

## Critical prompts (what this function thinks about)
> Why do we need a partner?
> Why would they need us?
> What does each side contribute?
> What does each side gain?
> What makes this strategically valuable?
> What capabilities does the partner possess?
> What capabilities do we possess?
> Who actually owns the relationship?
> Who decides?
> Who can block?
> What incentives are misaligned?
> What must be true for this partnership to work?
> What are the failure conditions?
> What is the smallest proof of value?
> What should we negotiate?
> What should we not negotiate?
> Should we invest more?
> Should we restructure?
> Should we expand?
> Should we exit?

## Canonical record schema (Learning Ledger + Decision Object Fields)
Every decision in this line is recorded as:
- a **Decision Object** — see `schema/decision-object.json`
- a **Learning Ledger** entry — see `schema/learning-ledger.json`

and the agent must run the **Orientation Protocol** first (see `AGENT.md`).

## How this line runs on SYNAPSIS (the cognitive substrate)
Every decision in this line is decomposed through the shared SYNAPSIS transformation
chain ([`00-kojiki-ontology/synapsis`](https://github.com/robfuj/kojiki-ontology/synapsis)):
```
SOURCE → RECORD → EVIDENCE → INTERPRETATION → STRATEGY → INTERACTION → OUTPUT → OUTCOME → LEARNING
```
- **Three steps are dedicated niche bots**: `bots/evidence/` (this line's extraction
 specialist); the shared `synapsis/audit-bot/` (independent audit, org-wide) and
 `synapsis/learning-bot/` (cross-line memory). See `AGENT.md` for the full contract.
- The rest run inline inside this line's agent, each bounded to one authority.
- Meta-rule: *evidence ≠ interpretation ≠ belief ≠ doctrine.* Validate with
 `python3 synapsis/validate.py <record.json>` (in the ontology repo).

## How to use
1. Read `AGENT.md` — the first-run Orientation Protocol.
2. Read `SCHEMA.md` — how this line maps to the universal schema.
3. Read `data/05-business-development.json` — the machine-readable spec.
4. See `data/example.json` — one fully worked decision (Decision Object + Ledger).
5. Use `decision-graph.mmd` — agent-decodable operating tree + state model.
6. Validate new records: `python3 tools/validate.py data/<name>.json`
