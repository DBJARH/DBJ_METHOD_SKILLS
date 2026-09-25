---
title: dbj-taxonomy
weight: 1
---

# dbj-taxonomy

Where does a concern sit? (4 Categories × 4 Capabilities)

DBJ.METHOD Enterprise Taxonomy — the official two-level Category/Capability
hierarchy for classifying enterprise concerns. Use whenever DBJ asks to
classify, position, or map a concern, role, system, or document within his
enterprise architecture; whenever discussing Conceptual/Logical/Physical/Implementation
layers; whenever distinguishing Taxonomy Capability (structural) from
Organizational Capability (measurable); or whenever DBJ references "the
taxonomy", "BPT", "DBJ ADM", or method.dbj.org content.

## DBJ Enterprise Taxonomy

Authoritative source: [method.dbj.org/taxonomy_core.html](https://method.dbj.org/taxonomy_core.html) — single source of truth
for the hierarchy and terminology, to be used with no changes or reinterpretations.
Explanatory companion (non-authoritative): [method.dbj.org/taxonomy](https://method.dbj.org/taxonomy)

Verified 2026-06-30: core and explanatory page are consistent — same 4 Categories,
same 16 Capabilities, no additions/deviations in core. If they ever diverge, core wins.

### Core shape

Two-level hierarchy: 4 Categories, each with 4 Capabilities (16 total).
Categories are ordered top (most abstract) to bottom (most concrete).

| Category | Capabilities |
|---|---|
| Conceptual | Business, Information, Application, Technology |
| Logical | Data Management, Integration, Platform, Security |
| Physical | Compute, Infrastructure, Network, Storage |
| Implementation | Deployment, Development, Monitoring, Operations |

- Conceptual — blueprint: business goals, info domains, app functions, tech choices.
- Logical — design: component interaction, data governance, integration, security.
- Physical — tangible resources: hardware, infra, connectivity, storage.
- Implementation — build/run practices; lower layers = more engineering roles, but architectural decisions on structure/boundaries apply at every level.

### Capability — two facets (do not conflate)

1. Taxonomy Capability (Structural) — fixed named node, defined only by taxonomy_core. Doesn't change with staffing/time/maturity.
2. Organizational Capability — the measurable ability to staff/execute within that node. Variable, basis for enterprise KPIs.

"Business capability" (singular industry term) is NOT a Taxonomy term — it belongs to the Business Landscape layer and maps across one or more Taxonomy nodes.

### Roles vs Capabilities

- Roles (Product Owner, EA, BA, Stakeholder) are organizational, not Taxonomy terms.
- A Role's Actors collectively own ability within one or more Capabilities.
- Actors need not be human — can be system/service/automated process depending on POV.
- Example: EA and BA both serve the "Business" Capability under "Conceptual" — same Capability, different Roles.

### Usage rules when applying this skill

- All 16 node names are official terminology — use verbatim, no rephrasing, no reinterpretation.
- Root of the tree is top-left (Conceptual/Business first).
- Taxonomy is a precondition for climbing CMM Levels (see [method.dbj.org/cmm](https://method.dbj.org/cmm)).
- When classifying something DBJ describes, locate it as Category → Capability, and state explicitly which of the two Capability facets (structural slot vs organizational maturity) is in play if relevant.
- If DBJ's request touches Business/Product/Technology segmentation, note the BPT Operational Model KB section is the related-but-distinct layer (method.dbj.org/kb/BPT_Operational_Model) — don't merge BPT segments with Taxonomy Capabilities.

See also: [dbj-bpt]({{< relref "dbj-bpt" >}}), [dbj-cmm]({{< relref "dbj-cmm" >}}), [dbj-adm]({{< relref "dbj-adm" >}}).
