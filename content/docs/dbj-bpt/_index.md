---
title: dbj-bpt
weight: 2
---

# dbj-bpt

Who owns delivery? (Business → Product → Technology loop)

DBJ.METHOD B-P-T (Business-Product-Technology) Operating Model — the
continuous delivery loop, the four Activity Streams, and how it relates to
DBJ ADM and Taxonomy. Use when DBJ discusses the BPT loop, business/product/technology
segmentation, role jurisdictions, requirements flow between segments, or asks
how a deliverable moves from business intent to implementation.

## DBJ B↔P↔T Operating Model

Authoritative source: [method.dbj.org/bpt.html](https://method.dbj.org/bpt.html)

### Disambiguation (do not conflate)

- BPT Loop = the mechanism — Business · Product · Technology cycle.
- Operating Model = its architectural role — what BPT is to the organization.
- BPT segments ≠ Taxonomy Categories/Capabilities (see [dbj-taxonomy]({{< relref "dbj-taxonomy" >}})). Different layer.

### The Loop

- Business — market strategy, stakeholders, owners — declares intent.
- Product — spec & delivery management — decouples Business/Technology so each evolves independently, while keeping delivery coherent and traceable.
- Technology — engineering/dev — implements to product specifications.

Each segment has its own logical repository for deliverables. The DBJ ADM
wheel places deliverables into the correct repository; roles watch their
domain repository, never the wheel directly — this decoupling is deliberate.

ADM-to-segment mapping: Business produces Conceptual outputs. Product
produces Logical and Physical outputs. Technology receives Physical and
Implementation outputs (plus test material).

EA governs the loop from above — sets principles, governs transitions,
measures alignment. EA does not participate in delivery.

Entry ticket to the BPT Loop: DBJ CMM Level 5 (see [dbj-cmm]({{< relref "dbj-cmm" >}})).
*Caveat emptor: this threshold is stated on bpt.html only — cmm.html
itself doesn't restate it. Treat bpt.html as authoritative for this
specific figure and confirm with DBJ if precision matters.*

### Four Activity Streams

| Stream | Intent | Key Roles |
|---|---|---|
| Require | Business declares product needs; EA ensures strategic alignment | Business, EA |
| Develop | Technology builds to spec; EA governs coherence | Technology, Product, EA |
| Deploy | Product released to operations; EA validates compliance | Technology, Product, EA |
| Evaluate | Measure outcomes vs. objectives; feeds back into Require | Business, Product, EA |

Evaluate → Business → Require: the loop never stops.

### Relationship to other DBJ.METHOD layers

- DBJ ADM wheel runs as governance layer above BPT, producing what the three segments consume — see [dbj-adm]({{< relref "dbj-adm" >}}).
- CMM Level 5 is precondition for smooth BPT cycling — see [dbj-cmm]({{< relref "dbj-cmm" >}}).
- Taxonomy Categories (Conceptual/Logical/Physical/Implementation) classify where a deliverable sits; BPT segments classify who owns it — see [dbj-taxonomy]({{< relref "dbj-taxonomy" >}}).

### Usage rule

- "Product" here is always the BPT segment (spec/delivery alignment), not a software product — disambiguate if DBJ's phrasing could mean either.
