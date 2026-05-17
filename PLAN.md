# Summer Book Report — Builder Sabbatical (Feb 8 – May 17, 2026)

**v2 plan — Codex critique incorporated.**

---

## Thesis (Editorial Spine)

> *Ninety-nine days. One person on medical leave decided to turn himself into an agent-orchestration laboratory. He shipped less product than he hoped. But he came out the other side running a multi-machine squad of named AI agents, having invented a handful of small protocols, and with an operating system for how to think about building in 2026. This is the field report.*

## Audience

**Public.** Friends, future collaborators, peers in the agent-tooling space. Murch will share the link openly.

**Redactions for public version:**
- Tailscale IPs → "private mesh"
- Hostinger VPS IPs → "the VPS"
- Airtable base IDs → "the Airtable"
- Linear ticket IDs → drop or generalize
- Domestic/medical details → keep at the level of memoir, never operational
- FMLA case details → omit specifics
- Spouse/family names → first name only with consent assumed

## Constraint: "Canonical Enough"

Don't repair the world. Snapshot "as-of-2026-05-17" with sources labeled. Where Airtable and TRACKER disagree, note the discrepancy in the report itself — transparency beats false precision.

---

## Source Citation Model

Every number gets a tag in superscript or `data-source`:
- `[A]` Airtable
- `[T]` TRACKER.md
- `[G]` Git log
- `[D]` Diary / journal narrative
- `[E]` Estimate (caveat shown)

---

## Revised Iteration Plan

### Iter 1 ✓ — Discovery + plan + codex critique
- Inventoried prior artifacts
- Wrote PLAN.md, dispatched codex
- Confirmed tooling: vercel, gemini, codex, aider all available
- **Key data points locked:** 94 idea folders, 93 unique IDs, 1 collision (#74), 2,681 commits across 13 repos Feb 8–May 17

### Iter 2 (now) — Deploy skeleton + visual system
- Stand up `journal/v2/deploy/index.html` with bare skeleton
- `vercel --prod` to get URL early
- Establish design system: type scale, palette, grid, components

### Iter 3 — Outline + freeze data snapshot
- `src/outline.md` with section list + thesis
- `data/snapshot-2026-05-17.json` with numbers + sources

### Iter 4 — Draft content (Hero → By the Numbers → Squad → Products)
### Iter 5 — Continue content (Concepts Learned → Invented → Tools → Honest Accounting → Skills → Closing)
### Iter 6 — Add one strong systems map + timeline diagram + 2-3 inline charts
### Iter 7 — Mobile / print / accessibility QA, redeploy
### Iter 8 — Content adversarial review (1 reviewer, single pass)
### Iter 9 — Visual/code review + final pass
### Iter 10 — Verify live, polish, ShipIt!

---

## Sections (10, editorial order)

1. **Prologue: 99 Days** — opening, FMLA context, thesis
2. **By the Numbers** — corrected stats, sourced
3. **The Squad** — agents by role/machine/capability/failure mode (operational table + sketch)
4. **Products** — Tangent, Naggler, Career Mode, Tender/Lume, Promptrait, ES Scalper, Caddy+RefClaw orchestration, Business Ideas portfolio
5. **Concepts I Learned** — RAMS, peer-approval protocols, Mem0, diverge-converge, TokenRouter ladder
6. **Concepts I Invented (or at least named first)** — voice exhaust training, peer-approval mesh, agent ecology with named identities, Caddy-as-shaper, RAMS-from-postmortems, PS5 controller programming experiment
7. **Tools in the Stack** — one systems map; not 40 stat cards
8. **Skills Developed** — squad orchestration, embeddings infra, cross-machine sync, exec governance, agent design
9. **Honest Accounting** — abandoned repos, $0 revenue, doc:code ratio, what didn't ship
10. **What's Next** — going back to Visa, what stays, what gets killed

---

## Design Direction (Reframed)

**Goal:** editorial, technically dense, honest. Not faux-literary Substack. Not corporate dashboard.

- **Type:** Fraunces (display serif) + Inter (body sans) + JetBrains Mono (numerals/code). Single bold expressive opener, then dense readable body.
- **Palette:** Paper `#F5F1E8`, ink `#1A1714`, accent `#9C3A1F` (oxblood — restrained, not ochre); secondary `#4A5240` (sage-ink). Inverse section for the squad (dark olive paper, cream ink) — *one* dramatic shift, not multiple.
- **Layout:** narrow single-column main column (~620px), wide margins where annotations/sources live (like editorial endnotes). Numbered chapter dividers. Drop caps only on the prologue.
- **Diagrams:** one precise systems map (squad topology, redacted). One timeline. ~3 inline data viz (commits-by-week, idea-counts, tool-categories). All SVG, hand-tuned, not Chart.js defaults.
- **Motion:** none on load. Scroll progress bar. Print stylesheet mandatory.
- **Accessibility:** WCAG AA, semantic HTML, alt text, skip-link.

---

## Definition of Done (revised)

1. Live Vercel URL — published on Iter 2, polished by Iter 10
2. All 10 sections present
3. Numbers sourced
4. Privacy redactions applied
5. ≥1 systems map + ≥1 timeline + ≥3 inline viz
6. Mobile + print pass
7. ≥1 external adversarial review acted on
8. `ShipIt!` only when the page reads well, looks elevated, and the URL is live
