## 2026-09-21T00:00:00Z - Civo Navigate script adaptation

### Goal

Create an independent Civo Navigate 2026 working copy of the Agent Craft deck, then map the supplied infrastructure-focused script into Slidev presenter notes without prematurely completing the new visual design.

### Changes

- Copied the editable Slidev source, components, styles, assets and project configuration from `~/Sites/_keynotes/agent-craft-2026`.
- Excluded source Git metadata, installed dependencies, virtual environments and generated `dist` output.
- Expanded the deck from 30 to 45 slides so every major new evidence beat has its own presenter-note boundary.
- Replaced all inherited presenter notes with the Civo script and synchronized `script.md` from those notes for rehearsal.
- Added lightweight evidence placeholders for the crypto ask, Meta Sentinel, the nine-second deletion, Jer Crane's post-mortem, Steve Yegge's rules, Origin, commit identity, Buzz, kagent, the Bubbles epilogue and OpenClaw memory inspector.
- Swapped the closing autonomy and values beats into the order used by the new script.
- Updated package and README identity for Civo Navigate 2026.

### Decisions

- Kept the original deck's components and visual grammar so the design pass can iterate rather than rebuild.
- Used visible `SBPlaceholder` frames for missing evidence. This preserves sequence, aspect-ratio intent and presenter notes while making unfinished sourcing explicit.
- Kept stage directions and optional hand-off markers in the notes because the talk is tomorrow and those choices still depend on the live programme and speaker experience.
- Treated `slides.md` as the canonical script; `script.md` is a rehearsal copy, not a second independently edited source.

### Tradeoffs

- New evidence slides are structurally ready but intentionally under-designed.
- The source repository's `.git` directory was not copied, avoiding accidental pushes to the Agent Craft remote. This working directory is not yet a Git repository.
- A targeted primary-source check covered Meta Muse, the EU AI Act sentence, the Bank of England quote and OpenClaw 2.0. The rest of the time-sensitive evidence still needs verification.
- `npm audit fix` was not run because it could introduce dependency changes immediately before the talk.

### Risks

- The 5,576-word script is approximately 38 minutes at 145 words per minute before pauses, audience interaction and laughter; confirm the slot length before the design pass.
- Presenter choices remain at `[ADJUST]` and `[YOUR ...]` markers, including the Warp line, OpenClaw 2.0 experience and EU AI Act expansion.
- Several high-specificity claims listed in `docs/source-check.md` still need primary-source verification and evidence capture before presentation.
- `npm install` reports 16 dependency vulnerabilities: 7 moderate and 9 high.
- Newly added evidence slides currently contain labelled placeholders rather than final screenshots.

### Verification

- `npm install` completed successfully.
- `npm run build` completed successfully with Slidev 52.16.0.
- `npm run export:png` exported all 45 slides.
- A 45-slide montage was reviewed for sequence and obvious render failures; all slides rendered and the intended placeholders are visible.
- The deck contains 45 presenter-note blocks, one per slide.

### Demo Impact

The talk now reads as an infrastructure field report: it moves from Bubbles' credentials and blast radius through least privilege, agent factories, workload identity, auditability and in-cluster agents, then closes by treating agents as infrastructure rather than productivity add-ons.

### Customer-Facing Context

The strongest enterprise thread is bounded autonomy backed by infrastructure controls: identity, scope, logs, independent backups and provable action history. The deck explicitly separates prompt-level instructions from constraints that must be enforced outside the model.

### Next Recommended Step

Confirm timing and resolve the four presenter-only choices, then source and fact-check the new evidence in narrative order before designing the placeholder slides.
