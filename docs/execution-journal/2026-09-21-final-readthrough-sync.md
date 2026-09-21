# Final read-through sync

## Outcome

Aligned the Civo Navigate deck with the final 21 September read-through script and review punch list. The deck is now 39 slides, with presenter notes and `script.md` mechanically synchronized.

## Decisions

- Split the chief-of-staff story onto its own evidence slide using Nick's real demo capture.
- Added a four-field-stop route slide and a four-question hallway slide because both are explicit spoken beats that benefit from on-screen structure.
- Kept diagrams for the timeline, task/system comparison and architecture; used screenshots, quotes and single-line statements for stories.
- Replaced the Jer, Project Mirror, Origin and Buzz evidence with the supplied Downloads assets, converted to compact WebP files for reliable conference loading.
- Simplified the OpenClaw memory slide to one line and removed the obsolete “think in systems” closing slide.
- Reordered the closing to question shift → autonomy → infrastructure treatment → Code Club → hallway questions → contact.
- Kept the agent-authorship joke at the end of the spoken close and increased the global footer's contrast and size.
- Restyled the Sparkle Bureaucracy panel with Inter-family typography, a dark surface and pink-to-teal accents matching the site.

## Verification

- `slides.md` contains 39 presenter-note blocks and no bracketed stage annotations.
- `script.md` exactly matches the 39 canonical note blocks.
- `npm run build` succeeds.
- Exported and visually reviewed the revised evidence, route, close and contact slides as PNGs.

## Risk / fallback

- The Slidev build reports upstream Rolldown pure-annotation warnings from `@vueuse/core`; the build still succeeds.
- Keep the exported PDF as the offline venue fallback after deployment.
