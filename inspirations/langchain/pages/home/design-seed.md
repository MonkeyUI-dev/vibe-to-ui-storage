# Design seed — langchain/home

> Page-level candidate notes. **Default apply target is the product** (`langchain`). Use `--page` only when you intentionally want this page alone.
> Status: **preview only** — do not apply until the user confirms.
> Generated: 2026-07-25

## Page Context

- **Primary page type**: landing
- **Density**: <!-- low / medium / high — fill from full-scroll captures -->
- **Interaction model**: <!-- scrolling / scanning / ... -->
- **Design consequences**: Preserve hierarchy and density posture of a `landing` surface.
- **Kinds**: inferred / transferable

## Visual Direction

- Atmosphere drawn from `LangChain: Observe, Evaluate, and Deploy Reliable AI Agents` without cloning brand chrome.
- Prefer product-aware adaptation over literal restyling.
- **Kinds**: inferred / transferable

## Colors

| Role | Direction | Kind |
|------|-----------|------|
| Canvas / paper | Match value family from reference, not necessarily hex | transferable |
| Ink | High-legibility text color strategy | transferable |
| Emphasis / signal | Sparse attention color for evidence & CTAs | transferable |
| Brand identity hues | Do not copy | brand-specific |



## Typography

- Heading posture: <!-- fill from captures -->
- Body rhythm: <!-- line length / density -->
- Font hints observed: (none)
- **Kinds**: observed (hints) / transferable (scale & attitude) / brand-specific (proprietary faces)

## Motion

- See `motion.md` on this page; product seed should synthesize cross-page motion personality.

## Do’s and Don’ts

### Do
- Keep page-type fidelity first.
- Reuse transferable hierarchy, spacing rhythm, and evidence strategy.
- Require full-scroll coverage before claiming mid/lower-page observations.

### Don’t
- Auto-write project tokens or `DESIGN.md` from this seed.
- Copy logos, illustrations, or campaign photography.
- Force a landing-page hero onto a dense workbench (or the reverse) without explicit repositioning intent.

## Transferable rules

- Preserve page-type density and hierarchy logic before borrowing decorative detail. _(transferable)_
- Reuse color roles (surface / ink / emphasis) rather than copying brand-specific hex identities. _(transferable)_
- Do not transplant logos, mascots, or campaign photography. _(brand-specific)_

## Do not copy directly

- Brand marks, mascots, proprietary illustration systems
- Exact marketing copy and campaign layout lockups
- Page modules that only exist because of this product’s IA

## Apply gate

```bash
vibe-to-ui inspiration apply langchain --project <path>                 # product seed (default)
vibe-to-ui inspiration apply langchain --page home --project <path>
vibe-to-ui inspiration apply langchain --project <path> --confirm
```
