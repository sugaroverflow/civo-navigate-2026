<template>
  <div class="law-wrap">
    <div class="law-flow">
      <div class="law-node"><span>01</span><strong>constitution</strong></div>
      <i></i>
      <div class="law-node"><span>02</span><strong>courts</strong></div>
      <i></i>
      <div class="law-node"><span>03</span><strong>case law</strong></div>
      <i></i>
      <div class="law-node stop"><span>04</span><strong>work stops</strong></div>
    </div>

    <div class="law-grid">
      <section class="law-primary">
        <div class="law-kicker">THE FACTORY GOVERNED ITSELF</div>
        <div class="law-count">185</div>
        <div class="law-caption">rules in one file</div>
        <div class="rule-lines" aria-hidden="true">
          <span></span><span></span><span></span><span></span><span></span><span></span>
        </div>
      </section>

      <section class="law-stats">
        <div><strong>50+</strong><span>agents</span></div>
        <div><strong>10</strong><span>weeks</span></div>
        <div><strong>400</strong><span>rulings</span></div>
        <div><strong>650</strong><span>refusal points</span></div>
      </section>

      <section class="law-verdict">
        <span>FINAL RULING</span>
        <strong>No work was legal.</strong>
        <small>Admission controllers assume a human wrote the policy.</small>
      </section>
    </div>
  </div>
</template>

<style scoped>
.law-wrap {
  height: 100%;
  display: grid;
  grid-template-rows: auto 1fr;
  gap: 30px;
}

.law-flow {
  display: grid;
  grid-template-columns: 1fr 42px 1fr 42px 1fr 42px 1fr;
  align-items: center;
}

.law-flow i {
  height: 1px;
  background: var(--sb-line);
}

.law-node {
  display: flex;
  gap: 14px;
  align-items: center;
  padding: 14px 16px;
  border-top: 2px solid var(--sb-teal);
  background: oklch(94% 0.018 275 / 0.035);
}

.law-node span,
.law-kicker,
.law-verdict span {
  color: var(--sb-muted);
  font: 850 10px/1 "SFMono-Regular", Menlo, monospace;
  text-transform: uppercase;
}

.law-node strong {
  font-size: 17px;
}

.law-node.stop {
  border-top-color: var(--sb-pink);
}

.law-grid {
  min-height: 0;
  display: grid;
  grid-template-columns: 1.3fr 0.7fr;
  grid-template-rows: 1fr auto;
  gap: 20px;
}

.law-primary,
.law-stats,
.law-verdict {
  border: 1px solid var(--sb-line);
  background: oklch(18% 0.042 272 / 0.88);
}

.law-primary {
  grid-row: 1 / 3;
  position: relative;
  padding: 30px;
  display: grid;
  align-content: center;
  gap: 8px;
  overflow: hidden;
}

.law-count {
  color: var(--sb-yellow-soft);
  font: 900 116px/0.85 "Avenir Next", sans-serif;
  letter-spacing: -0.075em;
}

.law-caption {
  color: var(--sb-ink);
  font-size: 28px;
  font-weight: 820;
}

.rule-lines {
  position: absolute;
  right: 24px;
  bottom: 24px;
  width: 44%;
  display: grid;
  gap: 10px;
  opacity: 0.55;
}

.rule-lines span {
  height: 4px;
  background: var(--sb-yellow);
}

.rule-lines span:nth-child(2) { width: 82%; }
.rule-lines span:nth-child(3) { width: 94%; }
.rule-lines span:nth-child(4) { width: 68%; }
.rule-lines span:nth-child(5) { width: 88%; }
.rule-lines span:nth-child(6) { width: 58%; }

.law-stats {
  display: grid;
  grid-template-columns: 1fr 1fr;
}

.law-stats div {
  padding: 18px;
  display: grid;
  gap: 5px;
  border-right: 1px solid var(--sb-line);
  border-bottom: 1px solid var(--sb-line);
}

.law-stats strong {
  font: 900 31px/1 "SFMono-Regular", Menlo, monospace;
}

.law-stats span {
  color: var(--sb-muted);
  font-size: 12px;
  text-transform: uppercase;
}

.law-verdict {
  padding: 22px;
  display: grid;
  gap: 8px;
  border-left: 4px solid var(--sb-pink);
}

.law-verdict strong {
  color: var(--sb-pink-soft);
  font-size: 30px;
}

.law-verdict small {
  color: var(--sb-soft);
  font-size: 14px;
}
</style>
