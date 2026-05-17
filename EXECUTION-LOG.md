# 99 Days — Execution Log

**Started:** 2026-05-17 ~12:30 PT
**Finished:** 2026-05-17 ~13:20 PT (active RWL pass)
**Live URL:** https://99-days-five.vercel.app
**Source:** `/Users/murchewings/Projects/journal/v2/deploy/`

## Iterations

| # | Goal | Outcome |
|---|------|---------|
| 1 | Discovery + plan | Found prior dashboards (Feb 8–Mar 8 only). Wrote `PLAN.md`. Dispatched Codex adversarial review. |
| 2 | Codex critique applied | Pivoted: deploy skeleton early, public audience, source-cite numbers, "canonical-enough", editorial spine, redaction rules. |
| 3 | Vercel skeleton + facts | Deployed `99-days-five.vercel.app`. Locked snapshot: 99 days, 2,681 commits, 93 ideas, 9 agents, 44 skills. |
| 4 | Full content + HTML | Authored all 10 chapters in editorial structure: hero → numbers → squad → products → concepts learned/invented → stack → skills → honest accounting → next. |
| 5 | Visual QA round 1 | Caught: empty 4th slot in numbers grid; awkward dropcap; concepts grid layout bug. |
| 6 | Polish | Fixed grid to 4-col, larger dropcap with proper shape-outside, oxblood $0 quiet card. |
| 7 | One adversarial review (codex on live page) | Codex flagged: copy overclaims, Stack section is inventory not story, tiny mono labels, accessibility gaps, `.concepts p:nth-child(3)` bug. |
| 8 | Apply codex fixes | Softened "operating system" claim, "loaded chambers" → "paused", added prefers-reduced-motion + focus-visible, compressed Stack to 8-tool key, fixed concepts grid with `nth-of-type` + `grid-column: 2`, made tangent.my/naggler.com clickable. |
| 9 | Final visual QA | Desktop + mobile screenshots at 1440px and 390px. All chapters render. Systems map clean. Concepts list works. |
| 10 | Close out + ShipIt! | This log. |

## Key sources

- `~/Projects/journal/sabbatical-opus-review.md` — honest-accounting tone
- `~/Projects/journal/builder-sabbatical-recap-2026-02.md` — Feb diary
- `~/Projects/business-ideas/` filesystem — 94 dirs, 93 unique IDs, 1 #74 collision
- `~/Projects/claude-workflows/CADDY-*.md` — Caddy-as-shaper concept
- `~/Projects/claude-workflows/AGENT-TO-AGENT-APPROVALS.md` — peer-approval mesh
- Memory (`~/.claude/projects/-Users-murchewings-Projects/memory/`) — squad topology
- Git logs: 2,681 commits across 13 repos Feb 8–May 17

## Drift / open accounting

- Airtable Business Ideas (~93) vs TRACKER.md (73) vs filesystem (94 dirs / 93 nums) — flagged in Chapter IX of the report itself rather than reconciled.
- Token Dashboard (Airtable) — referenced as 73 services per memory; not patched.
- The report uses "canonical enough" instead of attempting bi-directional fixes. Documented honestly in chapter IX.

## Adversarial reviews

- Codex plan critique → `validation/codex-plan-critique.md`
- Codex page critique → `validation/codex-page-review.md`
- Gemini attempted (background) — failed mid-run on ripgrep fallback; skipped per codex's "one reviewer is enough" advice.

## Screenshots

All in `validation/screens/`:
- `FINAL-01-hero.png`, `FINAL-02-chapter1.png`, `FINAL-03-squad-redo.png`, `FINAL-04-map.png` (desktop 1440×900)
- `FINAL-M01-mobile-hero.png`, `FINAL-M02-mobile-numbers.png`, `FINAL-M03-mobile-inventions.png` (mobile 390×844)
- `07-numbers-fixed.png` after grid repair
- `10-stack-revised.png` after Stack compression
- `14-concepts-after.png` after concepts grid repair

## What I'd do differently

- Get a Linear-routed Factory Droid review for a fully async second-pair-of-eyes — but it would push past the 90-min envelope.
- Get a human user to read it before sharing widely.
- The voice-exhaust experiment is described as planned; once it actually ships a model checkpoint, update the report.
