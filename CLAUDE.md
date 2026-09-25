# CLAUDE.md

1. claude skills mapping/sourcing method.dbj.org
2. Make sure user scope claude.md is also read and obeyed `%USERPROFILE%\.claude\CLAUDE.md`
   1. pay special attention to Conversation protocol, in there
3. Published to https://skills.dbj.org/

## Document versioning

- Every markdown file **SHOULD** (not must) carry a decimal `version:` key in its front matter:

```yaml
---
version: 0.1
---
```

- `0.1` .. `1.0` — pre-releases leading up to release 1
- `1.1` .. `2.0` — releases 1.1 through 2.0
- and so on by the same pattern

SHOULD, not MUST: skip it where this repo forbids front matter, and where front matter already exists just add the `version` key without disturbing the rest.
