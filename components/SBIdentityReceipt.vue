<template>
  <div class="identity-wrap">
    <section class="commit-receipt">
      <div class="receipt-head">
        <span>COMMIT RECEIPT</span>
        <strong>8c31f2a</strong>
      </div>
      <div class="commit-title">fix: preserve actor identity across mirrored repos</div>
      <div class="identity-fields">
        <div><span>author</span><strong>Fatima Sarah Khalid</strong></div>
        <div><span>email</span><strong class="redacted">private.address@████████</strong></div>
        <div><span>signed by</span><strong>unavailable</strong></div>
        <div><span>submitted via</span><strong>Cursor Origin</strong></div>
      </div>
      <div class="receipt-foot">public repository · private metadata</div>
    </section>

    <section class="actor-stack">
      <div class="actor-heading">POSSIBLE ACTORS</div>
      <div class="actors">
        <div><span>01</span><strong>GitHub-me</strong></div>
        <div><span>02</span><strong>Cursor-me</strong></div>
        <div><span>03</span><strong>human collaborator</strong></div>
        <div><span>04</span><strong>agent</strong></div>
      </div>
      <div class="actor-verdict">
        <span>workload identity expects</span>
        <strong>one workload · one identity · one owner</strong>
      </div>
    </section>
  </div>
</template>

<style scoped>
.identity-wrap {
  height: 100%;
  display: grid;
  grid-template-columns: 1.16fr 0.84fr;
  gap: 38px;
  align-items: center;
}

.commit-receipt {
  border: 1px solid oklch(87% 0.13 92 / 0.42);
  background: oklch(18% 0.042 272 / 0.94);
  box-shadow: 0 26px 70px oklch(5% 0.025 270 / 0.28);
  transform: rotate(-0.5deg);
}

.receipt-head {
  min-height: 48px;
  padding: 0 18px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  border-bottom: 1px solid var(--sb-line);
  color: var(--sb-muted);
  font: 850 11px/1 "SFMono-Regular", Menlo, monospace;
}

.receipt-head strong {
  color: var(--sb-teal-soft);
}

.commit-title {
  padding: 25px 24px;
  border-bottom: 1px solid var(--sb-line);
  font-size: 24px;
  font-weight: 800;
}

.identity-fields {
  padding: 8px 24px;
}

.identity-fields > div {
  min-height: 58px;
  display: grid;
  grid-template-columns: 126px 1fr;
  gap: 18px;
  align-items: center;
  border-bottom: 1px solid var(--sb-line);
}

.identity-fields span,
.actor-heading,
.actor-verdict span {
  color: var(--sb-muted);
  font: 850 10px/1 "SFMono-Regular", Menlo, monospace;
  text-transform: uppercase;
}

.identity-fields strong {
  font-size: 16px;
}

.identity-fields .redacted {
  color: var(--sb-pink-soft);
  font-family: "SFMono-Regular", Menlo, monospace;
}

.receipt-foot {
  padding: 15px 24px;
  background: oklch(68% 0.18 344 / 0.08);
  color: var(--sb-pink-soft);
  font: 850 11px/1 "SFMono-Regular", Menlo, monospace;
  text-transform: uppercase;
}

.actor-stack {
  display: grid;
  gap: 15px;
}

.actors {
  border-top: 1px solid var(--sb-line);
}

.actors > div {
  display: grid;
  grid-template-columns: 42px 1fr;
  gap: 14px;
  align-items: center;
  padding: 16px 0;
  border-bottom: 1px solid var(--sb-line);
}

.actors span {
  color: var(--sb-yellow-soft);
  font: 850 11px/1 "SFMono-Regular", Menlo, monospace;
}

.actors strong {
  font-size: 20px;
}

.actor-verdict {
  padding: 18px;
  display: grid;
  gap: 9px;
  border-left: 4px solid var(--sb-yellow);
  background: oklch(87% 0.13 92 / 0.07);
}

.actor-verdict strong {
  color: var(--sb-yellow-soft);
  font-size: 17px;
}
</style>
