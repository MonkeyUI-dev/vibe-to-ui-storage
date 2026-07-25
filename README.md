# vibe-to-ui-storage

English | [简体中文](README.zh-CN.md)

**Design Context** storage for [Vibe-to-UI](https://github.com/MonkeyUI-dev). This repository holds cross-project brand language, design tokens, and platform adaptation rules for the local design companion to read and sync.

> **Build the dream you were told to put away.**

## What this is

This repository is not the Vibe-to-UI tool itself. It is the remote copy of its **Design Context Profiles**. Each profile describes the visual and narrative context for a brand, product, or client — not a specific output platform.

Profiles currently included:

| Profile | Description |
|---------|-------------|
| [`vibe-to-ui`](profiles/vibe-to-ui/) | Cross-platform brand master for the Vibe-to-UI product |

At runtime, profiles usually live at `~/.vibe-to-ui/profiles/<profile>/`. Use this repository for team sharing, version history, and backup.

## Directory structure

```
profiles/
└── vibe-to-ui/
    ├── profile.md      # Profile metadata and summary
    ├── brand.md        # Cross-platform brand master (visual language, principles, guardrails)
    ├── tokens.json     # Design tokens (W3C DTCG format)
    ├── decisions.md    # Design decision log (append-only)
    ├── sources/        # Extraction source records
    └── targets/        # Per-platform adaptation rules
        ├── github.md
        └── xiaohongshu.md
```

### File responsibilities

- **`profile.md`** — Profile identity, one-liner, available targets, and source summary.
- **`brand.md`** — Shared brand language: temperament, color story, typography, space and motion character, design principles, and guardrails.
- **`tokens.json`** — Machine-readable design tokens (colors, typography, spacing, radius, shadows, motion, etc.), following the [W3C DTCG Design Tokens Format](https://www.designtokens.org/).
- **`decisions.md`** — Design memory: what was decided, why, and which files it affects.
- **`targets/*.md`** — Platform adaptations on top of the shared brand (layout, hierarchy, artifact specs, etc.).
- **`sources/*.md`** — Original sources used for brand extraction and confidence notes.

## Brand snapshot (vibe-to-ui)

Vibe-to-UI is a local design companion for vibe-coding developers. It turns references, feelings, and product context into usable visual directions and reusable Design Context.

The visual system is **Dusty Pink Brutalist**:

| Role | Value | Use |
|------|-------|-----|
| Dusty Pink | `#DDCED2` | Structural canvas |
| Ink Black | `#121212` | Hierarchy, borders, hard shadows |
| Cool White | `#F8F9FA` | Working surfaces |
| Electric Blue | `#003BFF` | Primary actions and live state (accent only, never full-page fill) |

See [`profiles/vibe-to-ui/brand.md`](profiles/vibe-to-ui/brand.md) and [`profiles/vibe-to-ui/tokens.json`](profiles/vibe-to-ui/tokens.json) for full details.

## Usage

### Clone and browse

```bash
git clone https://github.com/MonkeyUI-dev/vibe-to-ui-storage.git
cd vibe-to-ui-storage
```

### Sync with a local profile

If you already use the Vibe-to-UI CLI locally, copy or link profiles from this repository into your local directory:

```bash
# Example: sync the vibe-to-ui profile locally
cp -r profiles/vibe-to-ui ~/.vibe-to-ui/profiles/vibe-to-ui
```

> **Note:** The frontmatter in `profile.md` marks the local copy as the live copy. Skill updates must not overwrite user profiles; this repository provides the seed/shared version.

### Platform adaptation rules

- GitHub README and documentation visuals → [`profiles/vibe-to-ui/targets/github.md`](profiles/vibe-to-ui/targets/github.md)
- Xiaohongshu covers and carousels → [`profiles/vibe-to-ui/targets/xiaohongshu.md`](profiles/vibe-to-ui/targets/xiaohongshu.md)

## Contributing

1. Log new decisions in `decisions.md` (append only; mark old entries as superseded instead of deleting them).
2. Update `brand.md` and `tokens.json` for brand-level changes; update the matching `targets/<platform>.md` for platform-level changes.
3. Do not commit secrets, credentials, or `.env` files (see [`.gitignore`](.gitignore)).

## License

[MIT License](LICENSE) — Copyright (c) 2026 MonkeyUI-dev
