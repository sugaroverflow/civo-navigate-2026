<template>
  <div class="buzz-wrap">
    <section class="channel-panel">
      <div class="channel-head">
        <span># INCIDENT / DEAD API KEY</span>
        <strong>4 signed participants</strong>
      </div>
      <div class="messages">
        <div class="message human">
          <div class="actor"><strong>fatima</strong><span>npub…41d</span></div>
          <p>Production calls are returning 401. Split the investigation.</p>
          <em>SIGNED</em>
        </div>
        <div class="message agent-a">
          <div class="actor"><strong>agent / trace</strong><span>npub…8ac</span></div>
          <p>Checking deployment history and secret rotation.</p>
          <em>SIGNED</em>
        </div>
        <div class="message agent-b">
          <div class="actor"><strong>agent / config</strong><span>npub…2f1</span></div>
          <p>Searching configuration drift across environments.</p>
          <em>SIGNED</em>
        </div>
        <div class="message agent-c">
          <div class="actor"><strong>agent / verify</strong><span>npub…9b7</span></div>
          <p>Found stale key reference. Verifying replacement.</p>
          <em>SIGNED</em>
        </div>
      </div>
    </section>

    <section class="governance-panel">
      <div class="governance-item good">
        <span>AFTER THE FACT</span>
        <strong>Who did what?</strong>
        <p>Visible, persistent and cryptographically signed.</p>
      </div>
      <div class="governance-item gap">
        <span>RIGHT NOW</span>
        <strong>What are they doing?</strong>
        <p>Open every harness log, one agent at a time.</p>
      </div>
      <div class="governance-rule">Control is not proof. Proof is not observability.</div>
    </section>
  </div>
</template>

<style scoped>
.buzz-wrap {
  height: 100%;
  display: grid;
  grid-template-columns: 1.2fr 0.8fr;
  gap: 30px;
}

.channel-panel {
  border: 1px solid oklch(70% 0.155 304 / 0.46);
  background: oklch(18% 0.042 272 / 0.9);
  min-height: 0;
  transform: rotate(-0.25deg);
}

.channel-head {
  min-height: 48px;
  padding: 0 16px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  border-bottom: 1px solid var(--sb-line);
  font: 850 10px/1 "SFMono-Regular", Menlo, monospace;
}

.channel-head span {
  color: var(--sb-purple-soft);
}

.channel-head strong {
  color: var(--sb-muted);
}

.messages {
  padding: 15px 20px;
  display: grid;
  gap: 8px;
}

.message {
  position: relative;
  display: grid;
  grid-template-columns: 132px 1fr;
  gap: 16px;
  align-items: center;
  padding: 14px 72px 14px 14px;
  border-left: 2px solid var(--sb-teal);
  background: oklch(94% 0.018 275 / 0.035);
}

.message.human {
  border-left-color: var(--sb-pink);
}

.actor {
  display: grid;
  gap: 5px;
}

.actor strong {
  font-size: 13px;
}

.actor span,
.message em,
.governance-item span {
  color: var(--sb-muted);
  font: 800 9px/1 "SFMono-Regular", Menlo, monospace;
  font-style: normal;
  text-transform: uppercase;
}

.message p {
  color: var(--sb-soft);
  font-size: 14px;
  line-height: 1.3;
}

.message em {
  position: absolute;
  right: 12px;
  color: var(--sb-teal-soft);
}

.governance-panel {
  display: grid;
  align-content: center;
  gap: 15px;
}

.governance-item {
  min-height: 145px;
  padding: 22px;
  display: grid;
  align-content: center;
  gap: 9px;
  border-top: 3px solid var(--sb-teal);
  background: oklch(77% 0.115 190 / 0.07);
}

.governance-item.gap {
  border-top-color: var(--sb-yellow);
  background: oklch(87% 0.13 92 / 0.07);
}

.governance-item strong {
  font-size: 28px;
}

.governance-item p {
  color: var(--sb-soft);
  font-size: 15px;
  line-height: 1.35;
}

.governance-rule {
  padding: 18px;
  border-left: 4px solid var(--sb-pink);
  color: var(--sb-pink-soft);
  font-size: 17px;
  font-weight: 800;
  line-height: 1.3;
}
</style>
