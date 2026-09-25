---
title: dbj-adm
weight: 4
---

# dbj-adm

How are decisions authorized? (5-step governance wheel)

DBJ ADM — the simplified 5-step architecture governance wheel (Principles,
Vision, Architecture, Decision, Governance), adapted from TOGAF ADM's 9
steps, plus Requirements Management traceability. Use when DBJ discusses
architecture deliverables, the ADM wheel/steering wheel metaphor,
requirement traceability (REQ-IDs), or governance cycles for a specific
initiative.

## DBJ ADM

Authoritative source: [method.dbj.org/kb/DBJ_ADM/](https://method.dbj.org/kb/DBJ_ADM/)
Simplified version of TOGAF ADM. The wheel authorizes delivery; it never
delivers — outputs are always architectural artifacts (decisions,
principles, constraints, blueprints), never deployed systems or running
code.

Precondition: organization at DBJ CMM Level 3+ (see [dbj-cmm]({{< relref "dbj-cmm" >}})) — ensures the org can actually "steer the wheel."

### Five steps (TOGAF's 9 steps reduced to 5)

| Step | Taxonomy Category(ies) |
|---|---|
| 1 — Principles | Conceptual |
| 2 — Vision | Conceptual |
| 3 — Architecture | Conceptual → Logical → Physical |
| 4 — Decision | Implementation |
| 5 — Governance | Implementation |

(Taxonomy Categories per [dbj-taxonomy]({{< relref "dbj-taxonomy" >}}) skill.)
Each step produces ≥1 written artifact; the Architecture Board reviews
artifacts, not conversations.

### Mandatory deliverables (one per step)

1. Principles document — constraints/non-negotiables governing the wheel
2. Architecture Vision — business case, scope, stakeholder sign-off
3. Architecture definition — full cross-category Conceptual→Physical
4. Decision record — approved path forward, sequencing, cost
5. Governance report — compliance verification, loop closure

Other TOGAF deliverable types (Capability Maps, Application Portfolio
Catalogs, etc.) are optional — produce only what's needed to answer the
business question at that step.

### Requirements Management

Central, continuous, persistent store — not a step. Usually maintained
org-wide, not per-project. Every ADM step reads current requirements
relevant to it; unresolved concerns at one Taxonomy Category are logged
and picked up at the right step rather than dropped.

Traceability: each deliverable references the REQs it satisfies; REQs may
reference other REQs, forming an auditable dependency graph back to the
originating Conceptual declaration. This traceability is the mechanism
behind DBJ CMM Level 5 (self-improving, measurable process).

If DBJ's org already has established requirements tooling/practice, that
takes precedence — DBJ ADM integrates with it; only the traceability
principle must be preserved.

### One wheel or many

- Single wheel: appropriate for small orgs / simple landscapes / narrowly scoped engagements.
- Multiple concurrent wheels: each independently scoped and governed; EA coordinates so Conceptual outputs don't conflict across wheels.
- A wheel scoped purely to Conceptual outcomes (e.g. a standards review) may close without triggering Product or Technology BPT segments at all — that's a valid, complete outcome.
- Structure never changes regardless of scale: every wheel follows the 5-step structure, uses REQ traceability, and lands deliverables in the correct BPT repository (see [dbj-bpt]({{< relref "dbj-bpt" >}}) skill).

### Relationship to BPT

DBJ ADM is the governance layer; BPT Operating Model is what consumes its
deliverables across the three segments. ADM authorizes; BPT delivers. See
[dbj-bpt]({{< relref "dbj-bpt" >}}) skill for the segment mapping.
