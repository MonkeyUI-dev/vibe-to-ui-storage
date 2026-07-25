# Design Decisions — Vibe-to-UI

> Append-only Design Memory for profile `vibe-to-ui`.
> Do not delete old entries. Mark superseded decisions instead.

## How to log

Each entry should answer: **what** was decided, **why**, and **what it affects** (brand master, tokens, a specific target, or assets).

---

## Log

### 2026-07-13 — Initial brand extraction

- **Decision**: Adopt the active Dusty Pink Brutalist system as Vibe-to-UI's shared brand language: dusty-pink canvas, ink-black structure, cool-white surfaces, and sparing electric-blue signals.
- **Why**: The product's local design specification and landing content consistently define this visual system and its creator-first tone.
- **Affects**: brand.md, tokens.json, targets/github.md, targets/xiaohongshu.md
- **Confidence**: high
- **Source**: sources/2026-07-13-local-design-context.md

<!--
### YYYY-MM-DD — Target web created

- **Decision**:
- **Why**:
- **Affects**: targets/web.md
- **Confidence**:
- **Source**:
-->

<!--
### YYYY-MM-DD — Superseded: previous accent

- **Decision**: Accent moved from #X to #Y
- **Why**:
- **Supersedes**: YYYY-MM-DD — Initial extraction (accent)
- **Affects**: tokens.json, targets/*
-->


### 2026-07-13 — Target github created

- **Decision**: Created stub targets/github.md
- **Why**: `vibe-to-ui context --target github`
- **Affects**: targets/github.md
- **Confidence**: n/a (lifecycle)
- **Source**: cli


### 2026-07-13 — Target xiaohongshu created

- **Decision**: Created stub targets/xiaohongshu.md
- **Why**: `vibe-to-ui context --target xiaohongshu`
- **Affects**: targets/xiaohongshu.md
- **Confidence**: n/a (lifecycle)
- **Source**: cli

### 2026-07-13 — GitHub and Xiaohongshu target rules formalized

- **Decision**: Use the shared Vibe-to-UI brand master for both platforms, adapting documentation hierarchy for GitHub and vertical creator-first storytelling for Xiaohongshu.
- **Why**: Each surface has different reading behavior, but neither requires a different brand token system.
- **Affects**: targets/github.md, targets/xiaohongshu.md
- **Confidence**: high
- **Source**: sources/2026-07-13-local-design-context.md
