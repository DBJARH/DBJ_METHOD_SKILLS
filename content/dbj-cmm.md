---
title: dbj-cmm
weight: 3
---

# dbj-cmm

Is the org ready? (5-element maturity scoring, L0–L5)

DBJ Capability Maturity Model (DBJ CMM) — organizational maturity scoring
across five structural elements (Governance, Skilled Resource Pool,
Projects/Portfolios, Business Operations, Architecture Repository) on an
L0-L5 scale. Use when DBJ asks to assess, score, or discuss organizational
maturity, readiness for BPT/ADM adoption, or CMM levels.

## DBJ Capability Maturity Model (DBJ CMM)

Authoritative source: [method.dbj.org/cmm.html](https://method.dbj.org/cmm.html)
Mirrors TOGAF CMM's scale/principle but scoped to the whole organization,
not just the EA practice.

### Five structural elements

- Governance — decision authority, policies, oversight
- Skilled Resource Pool — people and competencies
- Projects / Portfolios — how work is initiated, executed, delivered
- Business Operations — day-to-day function and continuity
- Architecture Repository — organizational knowledge base of decisions/patterns/principles

### Maturity scale (L0–L5)

| Level | Name | Description |
|---|---|---|
| L0 | None | No recognizable structure |
| L1 | Initial | Ad-hoc, person-dependent |
| L2 | Emerging | Processes being defined, inconsistently applied |
| L3 | Defined | Documented, standardized, consistently followed |
| L4 | Managed | Measured, monitored, actively controlled |
| L5 | Optimising | Continuous improvement embedded |

### Scoring rule — critical

Score each of the 5 elements independently. Organization level = the
MINIMUM score across all five — not an average. One weak element caps the
whole organization's rating.

Example: Governance=L4, Resource Pool=L3, Projects=L3, Business Ops=L2,
Repository=L3 → Organization level = L2.

### Thresholds that gate other DBJ.METHOD layers

- L3 across all five elements = entry ticket to DBJ ADM (org can host an Architecture Board, run the 5-step wheel, etc.) — see [dbj-adm]({{< relref "dbj-adm" >}}).
- L5 referenced as the entry ticket to the BPT Loop in bpt.html — see [dbj-bpt]({{< relref "dbj-bpt" >}}). (Note: cmm.html itself doesn't restate this figure; treat bpt.html as authoritative for that specific threshold and flag to DBJ if asked to confirm, since it's stated on a different page than the CMM definition.)

### Use when DBJ asks you to assess maturity

Walk through each of the 5 elements using their characteristics (4 per
element, listed on cmm.html — e.g. Governance: Decision Authority, Policy
Existence, Compliance Enforcement, Strategic Linkage) as evidence criteria,
score L0–L5 each, then report the minimum as the org-level score, naming
which element is the bottleneck.
