# Motion — langchain/home

> Live observation pass (load + full scroll + nav interaction). Confidence: **medium** — scroll-linked section reveals inferred from sticky sidebar; micro-interactions not fully instrumented.

## Observation checklist

- [x] Page load / entrance — hero headline glow present on first paint
- [x] Scroll / in-view reveals — left-rail platform sections highlight as bands enter view (Engine → Observability → Evaluation → Deployment → Fleet)
- [x] Hover / focus micro-feedback — nav dropdown chevrons; CTA pills invert/fill on hover (partial observation)
- [ ] Optional: tab / modal / drawer — customer carousel uses dot + arrow controls (not exercised)
- [ ] `prefers-reduced-motion` — not toggled in this pass

## Motion DNA

| Dimension | Notes | Confidence |
|-----------|-------|------------|
| Roles | **Guidance** (scroll-linked sidebar rail), **continuity** (dark→light band transitions), **feedback** (pill CTAs) | medium |
| Triggers | scroll / in-view for section rail; hover on nav + buttons | medium |
| Tempo | Moderate — marketing pace, not snappy app UI | medium |
| Easing character | ease-out on section cross-fades; no bounce | inferred |
| Density | **Selective** — glow on hero + diagram; restrained elsewhere | high |
| Signature motif | **Vertical lifecycle rail** — center/side spine with glowing node as you scroll product story | medium |
| Reduced motion | Likely simplifies glow/parallax; not verified | low |

## Transferable rules

- Use one **scroll-synced narrative device** (rail, stepper, or progress dot) on long landing pages instead of animating every block.
- Keep hero glow/entrance **once**; let mid-page breathe with static product UI captures.
- Carousel proof sections: prefer **manual arrows + dots** with subtle slide transition over auto-play marquees.

## Brand-specific (do not copy)

- LangChain lifecycle curve illustration animation
- Exact headline glow treatment and Webflow motion bundles
