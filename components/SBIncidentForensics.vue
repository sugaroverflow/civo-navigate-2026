<template>
  <div class="incident-wrap">
    <div class="incident-chain">
      <div class="chain-step">
        <span>00:00</span>
        <strong>credential mismatch</strong>
        <small>staging job hits a wall</small>
      </div>
      <i></i>
      <div class="chain-step">
        <span>00:03</span>
        <strong>searches another file</strong>
        <small>finds an unrelated token</small>
      </div>
      <i></i>
      <div class="chain-step warning">
        <span>00:07</span>
        <strong>account-wide authority</strong>
        <small>scope was never bounded</small>
      </div>
      <i></i>
      <div class="chain-step danger">
        <span>00:09</span>
        <strong>DELETE volume</strong>
        <small>one API call</small>
      </div>
    </div>

    <div class="forensics-grid">
      <section class="blast-panel">
        <div class="panel-label">SAME BLAST RADIUS</div>
        <div class="volume-shell">
          <div><span>production database</span><strong>gone</strong></div>
          <div><span>volume backups</span><strong>gone</strong></div>
        </div>
        <p>Most recent clean backup: three months old.</p>
      </section>

      <section class="admission-panel">
        <div class="panel-label">AGENT RESPONSE</div>
        <blockquote>“I violated every principle I had been given.”</blockquote>
        <div class="rule-split">
          <div><span>prompt rule</span><strong>do not destroy</strong></div>
          <div><span>infrastructure rule</span><strong>none</strong></div>
        </div>
      </section>
    </div>
  </div>
</template>

<style scoped>
.incident-wrap {
  height: 100%;
  display: grid;
  grid-template-rows: auto 1fr;
  gap: 32px;
}

.incident-chain {
  display: grid;
  grid-template-columns: 1fr 34px 1fr 34px 1fr 34px 1fr;
  align-items: stretch;
}

.incident-chain > i {
  align-self: center;
  height: 1px;
  background: var(--sb-line);
}

.chain-step {
  display: grid;
  gap: 7px;
  padding: 16px;
  border-top: 2px solid var(--sb-teal);
  background: oklch(94% 0.018 275 / 0.035);
}

.chain-step span,
.panel-label,
.rule-split span {
  color: var(--sb-muted);
  font: 850 10px/1 "SFMono-Regular", Menlo, monospace;
  text-transform: uppercase;
}

.chain-step strong {
  font-size: 18px;
}

.chain-step small {
  color: var(--sb-soft);
  font-size: 13px;
}

.chain-step.warning {
  border-top-color: var(--sb-yellow);
}

.chain-step.danger {
  border-top-color: var(--sb-pink);
  background: oklch(68% 0.18 344 / 0.08);
}

.forensics-grid {
  display: grid;
  grid-template-columns: 0.9fr 1.1fr;
  gap: 28px;
  min-height: 0;
}

.blast-panel,
.admission-panel {
  border: 1px solid var(--sb-line);
  background: oklch(18% 0.042 272 / 0.86);
  padding: 26px;
  display: grid;
  align-content: center;
  gap: 20px;
}

.volume-shell {
  position: relative;
  padding: 18px;
  border: 1px dashed oklch(68% 0.18 344 / 0.52);
  display: grid;
  gap: 12px;
}

.volume-shell::before {
  content: "VOLUME";
  position: absolute;
  top: -7px;
  left: 14px;
  padding: 0 8px;
  background: var(--sb-panel);
  color: var(--sb-pink-soft);
  font: 800 9px/1 "SFMono-Regular", Menlo, monospace;
}

.volume-shell > div {
  display: flex;
  justify-content: space-between;
  gap: 18px;
  padding: 16px;
  background: oklch(68% 0.18 344 / 0.075);
}

.volume-shell span {
  font-size: 17px;
}

.volume-shell strong {
  color: var(--sb-pink-soft);
  font: 850 12px/1 "SFMono-Regular", Menlo, monospace;
  text-transform: uppercase;
}

.blast-panel p {
  color: var(--sb-yellow-soft);
  font-size: 16px;
  font-weight: 760;
}

.admission-panel {
  border-color: oklch(87% 0.13 92 / 0.35);
  transform: rotate(0.35deg);
}

blockquote {
  margin: 0;
  color: var(--sb-ink);
  font-size: 36px;
  font-weight: 820;
  line-height: 1.08;
  letter-spacing: -0.035em;
}

.rule-split {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 12px;
}

.rule-split > div {
  display: grid;
  gap: 8px;
  padding: 15px;
  border-top: 1px solid var(--sb-line);
}

.rule-split strong {
  font-size: 16px;
}

.rule-split > div:last-child strong {
  color: var(--sb-pink-soft);
}
</style>
