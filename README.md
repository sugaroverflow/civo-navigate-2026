# Civo Navigate 2026 — The Agent Hype Is Real. So Is the Mess.

Talk for Civo Navigate 2026. A field report on what happens when agents meet infrastructure: credentials, blast radius, workload identity, auditability, agent-native forges, factories and fleets. Adapted from the Agent Craft 2026 keynote and expanded for a Kubernetes and infrastructure audience.

Built with [Slidev](https://sli.dev).

## Source

- `slides.md`: talk structure, slides, and presenter notes
- `script.md`: rehearsal copy mechanically synchronized from the presenter notes
- `components/`: reusable Slidev components (windows, stamps, nodes, placeholders)
- `styles/`: design tokens and slide primitives
- `public/assets/`: served event and logo assets
- `assets/`: original screenshot/photo source files

## Commands

```bash
npm run dev
npm run build
npm run build:pages
npm run export:png
npm run export:pdf
```

## Review Artifacts

- Static build: `dist/`
- Per-slide PNGs: `dist/png/`
- Optional Slidev PDF export: `dist/civo-navigate-2026.pdf`

## Placeholder Strategy

Every screenshot/evidence slot is represented as an `SBPlaceholder` with a label, optional replacement note, aspect ratio, and local image backing. Place real browser-safe assets under `public/assets/screenshots/`, keep original capture files under `assets/`, and update the `src` prop in `slides.md`. The newly added Civo evidence beats intentionally remain labelled placeholders until the design and sourcing pass.
