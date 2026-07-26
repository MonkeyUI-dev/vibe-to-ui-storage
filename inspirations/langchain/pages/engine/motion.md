# Motion — langchain/engine

> Live observation pass: load → scroll through feature bands → accordion click (Fix) → FAQ band review.

## Observation checklist

- [x] Page load / entrance
- [x] Scroll / in-view reveals / sticky / parallax
- [x] Hover / focus micro-feedback on primary controls
- [x] Accordion / tab content swap (Detect / Fix / Prevent stepper)
- [ ] `prefers-reduced-motion` behavior (not toggled in session — assume CSS media-query fallback standard)

## Motion DNA

| Dimension | Notes | Confidence |
|-----------|-------|------------|
| Roles | **continuity** (scroll narrative), **guidance** (timeline dot), **feedback** (accordion/CTA) | high |
| Triggers | scroll-in-view, accordion click/expand, hover on buttons/links | high |
| Tempo | **moderate** — neither snappy consumer-app nor cinematic landing | high |
| Easing character | **ease-out** on panel swaps; no bounce/spring | medium |
| Density | **selective** — motion concentrated in feature stepper + accordions, not ambient | high |
| Signature motif | **Vertical timeline dot** travels the center rail as Detect → Fix → Prevent sections activate; right panel cross-fades to matching product UI | high |
| Reduced motion | Panels should swap instantly or fade ≤150ms; disable dot travel | inferred |

## Observed behaviors

### Sticky navigation
- Nav bar remains fixed with subtle background blur as page scrolls from dark hero into light sections.
- Nav CTA buttons maintain static styling; no animated underline on links observed.

### Feature stepper (Detect / Fix / Prevent)
- **observed**: Clicking an accordion header (e.g. “Fix”) collapses the prior section and expands the next with content height animation.
- **observed**: Right-side product preview updates to match the active step — issue card → code diff/evaluator → prevention UI.
- **observed**: Center vertical rail dot aligns with the active section, implying scroll-sync or click-sync positioning.
- **inferred**: Scroll-driven activation likely also advances the active step as user scrolls through the band (common pattern for this layout).

### Hero
- Static on load — no staggered text entrance or particle animation observed in captures.
- Hero illustration appears fixed; no parallax separation between copy and graphic.

### FAQ accordion
- **observed**: Chevron rotation + height expand on question click (standard accordion).
- Tempo feels slightly faster than feature stepper — utilitarian, not decorative.

### Closing CTA band
- Decorative horizontal lines with blue dots appear static.
- Letter-spaced headline is typographic only — no per-character animation observed.

### Buttons / links
- **inferred**: Standard opacity or background shift on hover for primary/ghost buttons (Webflow/Framer typical).
- External-link CTAs include small arrow icon; no elaborate icon motion.

## Transferable rules

- For long-form B2B feature pages, invest motion budget in **one scroll-linked stepper** that swaps real UI evidence — not hero particle fields or fade-up-everything.
- Keep accordion transitions **≤300ms ease-out**; pair left narrative with right panel cross-fade so users perceive cause→effect.
- Avoid decorative motion in logo walls, FAQ, and footer — density is already low; motion would feel like SaaS template noise.
- Provide `prefers-reduced-motion: reduce` by showing final panel state without dot travel or height animation.

## Brand-specific (do not copy)

- Proprietary particle/generative art motion in resource thumbnails (if animated on hover — not confirmed)
- Any campaign-specific Lottie or mascot loops
