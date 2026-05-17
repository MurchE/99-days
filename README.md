# 99 Days — A Builder Sabbatical Field Report

A single-page editorial field report covering Feb 8 → May 17, 2026.

**Live:** https://99-days-five.vercel.app

## What's here

- [`deploy/`](deploy/) — the page itself (`index.html` + `style.css`). One HTML, one CSS, zero JS frameworks. Vercel-static.
- [`PLAN.md`](PLAN.md) — the 10-iteration Ralph Wiggum Loop plan used to build it. Incorporated codex critique after iter 1.
- [`EXECUTION-LOG.md`](EXECUTION-LOG.md) — what happened on each iteration.
- [`data/snapshot-2026-05-17.json`](data/snapshot-2026-05-17.json) — the canonical numbers + sources used in the report.
- [`validation/codex-plan-critique.md`](validation/codex-plan-critique.md), [`validation/codex-page-review.md`](validation/codex-page-review.md) — the two Codex CLI adversarial reviews acted on.
- [`validation/screens/`](validation/screens) — desktop + mobile screenshots from the build.

## Design

- Type: Fraunces (display serif), Inter (body sans), JetBrains Mono (numerals).
- Palette: paper `#F5F1E8` / ink `#1A1714` / oxblood accent `#8B2F1A` / one dark-olive inverse section for the squad.
- Layout: editorial single column. Numbered chapters. Source-tag superscripts on every number.
- Print + mobile stylesheets validated.

## Deploy

```sh
cd deploy
vercel deploy --prod
```

Set `outputDirectory: "."` in `vercel.json` (already configured) since there is no build step.

## License

CC BY 4.0 — share, adapt, attribute.
