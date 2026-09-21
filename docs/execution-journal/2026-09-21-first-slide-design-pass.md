## 2026-09-21T19:03:37Z - First Civo slide design pass

### Goal

Turn the new Civo script beats into a coherent first-pass deck, preserve the inherited field-report visual system, validate the result, and prepare a clean public GitHub repository.

### Changes

- Replaced the inherited Agent Craft title artwork and global event label with Civo Navigate-specific framing.
- Replaced the visible placeholder frames with native Slidev diagrams for the bio, crypto boundary, Sentinel comparison, destructive database incident, factory policy failure, Origin forge, commit identity, Buzz incident, kagent cluster repair, Bubbles recovery and OpenClaw memory inspector.
- Added ten reusable Vue components for those systems and evidence treatments.
- Restored the Project Mirror pipeline and fleet-assumption components so slides 27 and 29 explain the spoken argument rather than displaying unreadable screenshots.
- Reworked the closing infrastructure slide around four requirements: identity, scope, log and accountable owner.
- Added official/primary-source evidence assets for Meta Muse, Warp Factories, Cursor Origin, Buzz and the kagent field test under `public/assets/screenshots/civo/` with a source ledger in `docs/evidence-assets.md`.
- Updated the contact slide with Monday Merge and The Developer Show.

### Decisions

- Used native diagrams as the primary first-pass visual language. They expose the relationship the audience needs to understand at room scale; official screenshots are retained as source evidence and can become insets during the second pass.
- Marked the crypto correspondence as a reconstruction rather than presenting invented UI as an original screenshot.
- Chose `civo-navigate-2026` as the GitHub repository name. It matches the package name, Pages base path and export filename and is less likely to become stale than a title slug.
- Prepared the repository as public to match the inherited public keynote repository.

### Tradeoffs

- Several native diagrams summarize reported behaviour and are not substitutes for the speaker's own product captures.
- The first pass optimizes for narrative legibility, not pixel-perfect fidelity to Origin, Buzz, OpenClaw or kagent product UI.
- The OpenClaw memory slide remains a designed representation because no first-party screenshot is published and the speaker's own instance still needs a redacted capture.

### Risks

- RentAHuman statistics, the community-skill audit, Jer Crane's incident figures and Steve Yegge's factory figures still require primary-source confirmation before presentation.
- Speaker-owned captures are still needed for the exact Origin five-agent test, private-email metadata, Buzz API-key incident and OpenClaw memory UI.
- The script remains approximately 38 minutes before pauses.
- `npm install` reports 16 dependency vulnerabilities: 7 moderate and 9 high.

### Verification

- `npm run build` succeeds.
- `npm run build:pages` succeeds with the `/civo-navigate-2026/` base path.
- `npm run export:png` exports all 45 slides.
- Full-deck and targeted montages were reviewed after the component pass; the new slides render without visible overflow or clipping.
- A repository-readiness review found no obvious secrets, credentials or files above GitHub's 100 MiB limit.

### Demo Impact

The new middle of the talk now behaves as a systems narrative: credentials become blast radius; prompt rules are contrasted with infrastructure rules; fleet governance becomes identity plus observability; and the Bubbles epilogue returns to memory as inspectable infrastructure.

### Customer-Facing Context

The deck now has a concrete enterprise frame instead of a generic “trust” close. Agent systems are presented as unattended infrastructure that needs actor identity, bounded scope, action history and a named accountable owner.

### Subagent Review Notes

- The visual reviewer identified stale Agent Craft branding, empty evidence placeholders, weak Project Mirror/fleet explanations and an abstract final trust slide. Those recommendations were accepted and implemented.
- The evidence researcher sourced five official/primary visuals and documented their limitations. The assets were accepted; native diagrams remain the primary visuals for this first pass.
- The repository reviewer recommended `sugaroverflow/civo-navigate-2026`, public, and confirmed repository size, ignore rules, name availability and a clean secret scan. That recommendation was accepted.
- Deferred recommendations: redesigning the remaining inherited dense screenshots and reducing consecutive thesis slides. Those belong in the second pass after timing is confirmed.

### Next Recommended Step

Rehearse for timing, replace reconstructed evidence with speaker-owned captures where available, then do a final crop/annotation pass on the remaining inherited screenshots.
