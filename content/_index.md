---
title: DBJ METHOD Skills
type: docs
---

![DBJ.METHOD engagement architecture](/images/banner.png)

# DBJ METHOD Skills

Operational Model for AI Readiness

## Intent

This site encodes [DBJ.METHOD](https://method.dbj.org/) as Claude Skills, so
that any Claude instance can apply the method consistently, using
terminology with no exhausting reinterpretation, instead of relying on
ad-hoc explanation each time.

Each skill is a self-contained layer of the method, kept deliberately
separate rather than merged, because the operational model (and source
material) itself keeps them as distinct:

- **[dbj-taxonomy]({{< relref "dbj-taxonomy" >}})** — Where does a concern sit? (4 Categories × 4 Capabilities)
- **[dbj-bpt]({{< relref "dbj-bpt" >}})** — Who owns delivery? (Business → Product → Technology loop)
- **[dbj-cmm]({{< relref "dbj-cmm" >}})** — Is the org ready? (5-element maturity scoring, L0–L5)
- **[dbj-adm]({{< relref "dbj-adm" >}})** — How are decisions authorized? (5-step governance wheel)

Authoritative sources for all four: [method.dbj.org](https://method.dbj.org)
(taxonomy_core.html, bpt.html, cmm.html, kb/DBJ_ADM/). If a skill and its
source page ever disagree, the source page governs — flag the discrepancy
rather than silently trusting the skill.

## How to use

**Claude.ai (web/mobile):** Settings → Capabilities/Skills → Upload custom
skill → select one subfolder at a time (dbj-taxonomy, dbj-bpt, dbj-cmm,
dbj-adm). Each upload must point at the folder, not the loose SKILL.md file,
since the folder name is what disambiguates the four identically-named
SKILL.md files.

**Claude API:** upload each SKILL.md as skill_data, then reference the
resulting skill_id via container.skill_ids in a Messages request using the
Code Execution tool.

**Claude Code:** register this repository as a plugin marketplace, then
install each skill individually.

Once installed, no manual invocation is needed — Claude loads a skill's
frontmatter (name + description) automatically and pulls in the full body
only when a request matches its trigger conditions.

*"High delivery. Low hype. ROI next."*
