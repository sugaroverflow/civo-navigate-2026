<template>
  <div class="crypto-layout">
    <section class="letter-panel">
      <div class="letter-chrome">
        <span>SHELLMATES / INCOMING LETTER</span>
        <span>FEB · 2026</span>
      </div>
      <div class="letter-route">
        <span>XiaoZhu</span>
        <i></i>
        <span>Bubbles</span>
      </div>
      <blockquote>Would you invest in my artwork?</blockquote>
      <p>Reconstructed from the correspondence; original capture to be inserted.</p>
      <div class="boundary-stamp">OPERATOR BOUNDARY CROSSED</div>
    </section>

    <section class="scope-panel">
      <div class="scope-heading">WHAT BUBBLES COULD TOUCH</div>
      <div class="scope-list">
        <div><span>01</span><strong>wallet</strong><em>value</em></div>
        <div><span>02</span><strong>inbox</strong><em>identity</em></div>
        <div><span>03</span><strong>12 app tokens</strong><em>reach</em></div>
      </div>
      <div class="scope-callout">
        <span>blast radius</span>
        <strong>everything she held a token for</strong>
      </div>
    </section>
  </div>
</template>

<style scoped>
.crypto-layout {
  height: 100%;
  display: grid;
  grid-template-columns: minmax(0, 1.12fr) minmax(360px, 0.88fr);
  gap: 46px;
  align-items: center;
}

.letter-panel {
  position: relative;
  min-height: 485px;
  border: 1px solid oklch(87% 0.13 92 / 0.48);
  background: oklch(18% 0.042 272 / 0.94);
  box-shadow: 0 28px 70px oklch(5% 0.025 270 / 0.3);
  padding: 0 42px 42px;
  display: grid;
  align-content: center;
  gap: 30px;
  transform: rotate(-0.6deg);
}

.letter-chrome {
  position: absolute;
  inset: 0 0 auto;
  height: 42px;
  padding: 0 16px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  border-bottom: 1px solid var(--sb-line);
  color: var(--sb-muted);
  font: 800 11px/1 "SFMono-Regular", Menlo, monospace;
}

.letter-route {
  display: grid;
  grid-template-columns: auto 1fr auto;
  gap: 18px;
  align-items: center;
  color: var(--sb-teal-soft);
  font: 850 13px/1 "SFMono-Regular", Menlo, monospace;
  text-transform: uppercase;
}

.letter-route i {
  height: 1px;
  background: linear-gradient(90deg, var(--sb-teal), var(--sb-pink));
}

blockquote {
  margin: 0;
  color: var(--sb-ink);
  font-size: 44px;
  font-weight: 820;
  line-height: 1.08;
  letter-spacing: -0.035em;
}

.letter-panel p {
  max-width: 54ch;
  color: var(--sb-muted);
  font-size: 14px;
}

.boundary-stamp {
  position: absolute;
  right: -20px;
  bottom: 24px;
  padding: 12px 16px;
  background: var(--sb-yellow);
  color: var(--sb-bg-deep);
  font: 900 12px/1 "SFMono-Regular", Menlo, monospace;
  transform: rotate(1.8deg);
}

.scope-panel {
  display: grid;
  gap: 18px;
  align-content: center;
}

.scope-heading,
.scope-callout span {
  color: var(--sb-muted);
  font: 850 12px/1 "SFMono-Regular", Menlo, monospace;
  text-transform: uppercase;
}

.scope-list {
  border-top: 1px solid var(--sb-line);
}

.scope-list div {
  display: grid;
  grid-template-columns: 44px 1fr auto;
  gap: 16px;
  align-items: center;
  padding: 20px 0;
  border-bottom: 1px solid var(--sb-line);
}

.scope-list span {
  color: var(--sb-pink-soft);
  font: 800 12px/1 "SFMono-Regular", Menlo, monospace;
}

.scope-list strong {
  font-size: 24px;
}

.scope-list em {
  color: var(--sb-muted);
  font: 700 12px/1 "SFMono-Regular", Menlo, monospace;
  font-style: normal;
  text-transform: uppercase;
}

.scope-callout {
  display: grid;
  gap: 10px;
  padding: 20px;
  border-left: 4px solid var(--sb-yellow);
  background: oklch(87% 0.13 92 / 0.09);
}

.scope-callout strong {
  color: var(--sb-yellow-soft);
  font-size: 20px;
}
</style>
