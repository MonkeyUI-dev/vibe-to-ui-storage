# Design seed — langchain/engine

> Page-level candidate notes. **Default apply target is the product** (`langchain`). Use `--page` only when you intentionally want this page alone.
> Status: **preview only** — do not apply until the user confirms.
> Generated: 2026-07-26

## Page Context

- **Primary page type**: landing (product feature sub-page)
- **Secondary**: product-evidence showcase with scroll-linked narrative
- **Density**: medium-low
- **Interaction model**: vertical scroll, accordion feature stepper, FAQ expand, sticky nav
- **Design consequences**: Airy hero; real UI evidence in feature bands; dark→light→dark canvas rhythm; restrained selective motion
- **Kinds**: observed / transferable

## Visual Direction

- Premium dev-tool marketing: near-black technical hero, warm off-white mid-page, dark conversion/footer bookends
- Credibility through **embedded product UI** (issue cards, code, evaluators) not abstract SaaS illustrations
- Hairline grid rules instead of colored section blocks
- **Kinds**: observed / transferable

## Colors

| Role | Direction | Kind |
|------|-----------|------|
| Canvas dark | Near-black navy `#050A14`–`#0D1117` | observed / transferable |
| Canvas light | Warm off-white `#F5F3EF`–`#FAFAF8` | observed / transferable |
| Ink primary | Near-white on dark; near-black on light | observed / transferable |
| Ink secondary | Blue-gray `#8BA4C0` for labels/inactive | observed / transferable |
| Emphasis | Electric blue dots, timeline, pills — sparse | observed / transferable |
| CTA primary | White fill on dark; black fill on light | observed / transferable |
| CTA secondary | Ghost 1px hairline border | observed / transferable |
| Status (in UI previews) | Red severity, green tags — confined to evidence cards | observed / transferable |
| Brand identity | LangChain blue, parrot mark | brand-specific |

## Typography

- **Family**: Single geometric sans (grotesk/neutral); no serif pairing
- **Heading posture**: Large display H1 with soft blue-white tint on dark; bold black H3 on light sections
- **Body**: Regular weight, comfortable line-height (~1.5–1.6), max ~60ch in feature copy
- **Labels**: Small caps or semibold section headers; uppercase footer column titles
- **Signature**: Letter-spaced closing headline (one band only)
- **Kinds**: observed (attitude) / transferable (scale & hierarchy) / brand-specific (exact face)

## Space & Components

- **Buttons**: Full pill radius; consistent px-6 py-3-ish padding
- **Cards**: Rounded ~12–16px; dark gray fills; subtle glow for “embedded app”
- **Grid**: 8px-base spacing; large inter-section gaps (~80–120px)
- **Nav**: Sticky, translucent blur over scroll
- **Kinds**: observed / transferable

## Motion

- **Signature motif**: Vertical timeline dot on Detect→Fix→Prevent rail; right panel swaps with active step
- **Tempo**: Moderate ease-out (~200–300ms); no bounce
- **Density**: Selective — stepper + accordions only; static hero and logo band
- **Reduced motion**: Instant panel swap; no dot travel
- See `motion.md` for full DNA

## Page narrative beats

1. Hero position → 2. Logo trust → 3. Three-step capability (Detect/Fix/Prevent) → 4. Resources → 5. FAQ → 6. Closing CTA → 7. Footer

## Do's and Don'ts

### Do
- Use authentic product UI screenshots/cards for capability claims
- Keep accent color rare; lean on value contrast
- Insert FAQ before final CTA on dev-tool feature pages
- Preserve dark→light→dark pacing on long scrolls

### Don't
- Auto-write project tokens or `DESIGN.md` from this seed
- Copy LangChain logos, customer logos, or particle art
- Add cinematic hero animation or fade-up-everything
- Force this landing layout onto dense workbench surfaces

## Transferable rules

- Dark → light → dark canvas rhythm for B2B feature landings _(transferable)_
- Accordion stepper + live UI preview for complex product stories _(transferable)_
- Tiny accent budget; CTA polarity follows background value _(transferable)_
- FAQ before final conversion band _(transferable)_

## Do not copy directly

- LangChain / LangSmith marks and parrot icon
- Customer logo strip
- Proprietary particle generative thumbnails
- Exact copy and IA labels

## Apply gate

```bash
vibe-to-ui inspiration apply langchain --project <path>                 # product seed (default)
vibe-to-ui inspiration apply langchain --page engine --project <path>
vibe-to-ui inspiration apply langchain --project <path> --confirm
```
