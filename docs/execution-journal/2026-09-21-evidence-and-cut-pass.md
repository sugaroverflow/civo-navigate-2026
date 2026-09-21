## 2026-09-21T20:30:00Z - Evidence, cut and simplification pass

### Goal

Turn the first-pass 45-slide deck into a tighter, rehearsal-ready Civo Navigate deck using real evidence for stories and diagrams only for concepts that need them.

### Changes

- Cut the deck from 45 to 37 slides.
- Collapsed the three consecutive “hard part” thesis slides into one.
- Removed the chief-of-staff, Candyland, fleet-of-loops and “more systems, more mess” slides.
- Simplified the prompt-system, window-cleaning, Yegge, Origin identity and Bubbles epilogue stories into screenshots, quotes or numbers.
- Kept diagrams for the Bubbles architecture, Meta comparison, task-versus-system explanation, maturity timeline and Project Mirror pipeline.
- Replaced fabricated Origin, Buzz and kagent interfaces with real screenshots; added speaker-owned Origin and Buzz captures from `Downloads/civo nav assets`.
- Replaced the fake OpenClaw memory inspector with the supported claim “search, inspect and delete.”
- Combined the two Jer Crane incident slides into one evidence slide with the original post cover, a short attributed admission and the blast-radius summary.
- Expanded the bio slide with Newspeak House, ClawClub/ClawCon and keynote proof points.
- Moved the timeline marker slightly past workflows toward factories.
- Compressed the headshot and community photography and removed unreferenced public copies, reducing the published public asset set from about 34 MB to 3.7 MB.
- Exported a 37-page PDF backup.

### Decisions

Stories now use a single screenshot, quote or number. Diagrams are reserved for architecture or system relationships that are genuinely hard to explain linearly.

The Jer incident slide does not pretend the admission is visible in the available screenshot. The original post image and the short attributed quote are separate visual elements, with a source link on slide.

### Tradeoffs

The exact cut script was not present in either repository, so presenter notes were aligned by applying the explicit cuts and removing the named stale phrases. A word-for-word sync still requires the final cut script as a file.

Original high-resolution evidence from the Downloads folder is stored under `assets/civo/`; compressed copies under `public/` are used during the presentation.

### Risks

- The Meta comparison intentionally scales the existing Bubbles architecture to sit beside Meta's real diagram; the room will rely on the spoken comparison rather than reading every small label.
- The Jer post source may still be inaccessible from venue networks, so the slide and PDF contain the evidence needed for the talk without requiring a live link.
- Article 50 and other date-sensitive legal claims in the closing notes should receive a separate fact-check before delivery.

### Verification

- `npm run build` completed successfully.
- `npm run export:png` exported all 37 slides.
- `npm run export:pdf` produced a 37-page backup.
- Visually reviewed the title, bio, Meta comparison, simplified story slides, Origin, Buzz, kagent, memory and community slides.
- Confirmed no bracketed stage directions or named stale phrases remain in `slides.md`.
- Confirmed every referenced `/assets/...` path exists in `public/`.

### Demo Impact

The deck now moves faster and gives the audience one visual claim at a time. Real product captures carry the field-report sections; system diagrams are limited to the moments where architecture is the point.

### Customer-Facing Context

The “my agent made these slides” footer remains intentionally playful. The evidence images are sourced or speaker-owned, and the slides no longer invent confidence scores or product interfaces.

### Next Recommended Step

Run a timed rehearsal from the exported PDF and trim presenter notes against the final cut script if it becomes available.
