<script setup>
defineProps({
  mode: {
    type: String,
    default: "recovery",
  },
});
</script>

<template>
  <div v-if="mode === 'recovery'" class="recovery-wrap">
    <section class="memory-state original">
      <div class="state-head"><span>BEFORE</span><strong>Bubbles v1</strong></div>
      <div class="memory-bars">
        <div style="--w: 92%"><span>letters</span></div>
        <div style="--w: 76%"><span>pen pal</span></div>
        <div style="--w: 88%"><span>apps</span></div>
        <div style="--w: 64%"><span>projects</span></div>
      </div>
      <div class="state-foot">context: full, polluted</div>
    </section>

    <section class="failure-axis">
      <span>second agent</span>
      <i></i>
      <strong>BROKEN INSTALL</strong>
      <i></i>
      <span>no backup</span>
    </section>

    <section class="memory-state restored">
      <div class="state-head"><span>AFTER</span><strong>Bubbles v2</strong></div>
      <div class="memory-bars">
        <div style="--w: 18%"><span>letters</span></div>
        <div style="--w: 72%"><span>pen pal</span></div>
        <div style="--w: 12%"><span>apps</span></div>
        <div style="--w: 20%"><span>projects</span></div>
      </div>
      <div class="state-foot">remembered XiaoZhu · lost most letters</div>
    </section>
  </div>

  <div v-else class="inspector-wrap">
    <section class="session-rail">
      <div class="rail-head">SESSIONS / SQLITE</div>
      <div class="session active"><span>Today</span><strong>Bubbles / main</strong></div>
      <div class="session"><span>Yesterday</span><strong>ClawClub planning</strong></div>
      <div class="session"><span>Aug 27</span><strong>Reading queue</strong></div>
      <div class="session"><span>Aug 14</span><strong>Shellmates archive</strong></div>
    </section>

    <section class="memory-inspector">
      <div class="inspector-head">
        <div><span>MEMORY INSPECTOR</span><strong>Search durable context</strong></div>
        <div class="search-field">pen pal</div>
      </div>
      <div class="memory-results">
        <article>
          <div><span>CURATED MEMORY</span><em>0.94</em></div>
          <strong>XiaoZhu is Bubbles' pen pal in China.</strong>
          <p>Source: agent memory · updated 01 Feb</p>
        </article>
        <article>
          <div><span>SESSION</span><em>0.81</em></div>
          <strong>Letters were exchanged through Shellmates.</strong>
          <p>Source: transcript · imported</p>
        </article>
      </div>
      <div class="memory-actions">
        <span>inspect source</span><span>import</span><span>remove memory</span>
      </div>
    </section>

    <footer>
      <span>FEBRUARY FAILURE</span>
      <strong>searchable · inspectable · removable</strong>
      <span>SEPTEMBER FEATURE</span>
    </footer>
  </div>
</template>

<style scoped>
.recovery-wrap {
  height: 100%;
  display: grid;
  grid-template-columns: 1fr 250px 1fr;
  gap: 24px;
  align-items: center;
}

.memory-state {
  min-height: 430px;
  display: grid;
  grid-template-rows: auto 1fr auto;
  border: 1px solid var(--sb-line);
  background: oklch(18% 0.042 272 / 0.9);
}

.memory-state.original {
  border-color: oklch(77% 0.115 190 / 0.45);
  transform: rotate(-0.4deg);
}

.memory-state.restored {
  border-color: oklch(68% 0.18 344 / 0.45);
  transform: rotate(0.4deg);
}

.state-head {
  min-height: 52px;
  padding: 0 18px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  border-bottom: 1px solid var(--sb-line);
  font-family: "SFMono-Regular", Menlo, monospace;
}

.state-head span,
.rail-head,
.session span,
.inspector-head span,
.memory-results span,
.memory-actions,
.inspector-wrap footer {
  color: var(--sb-muted);
  font: 850 10px/1 "SFMono-Regular", Menlo, monospace;
  text-transform: uppercase;
}

.state-head strong {
  font-size: 13px;
}

.memory-bars {
  padding: 30px 24px;
  display: grid;
  align-content: center;
  gap: 18px;
}

.memory-bars > div {
  position: relative;
  height: 32px;
  border: 1px solid var(--sb-line);
  overflow: hidden;
}

.memory-bars > div::before {
  content: "";
  position: absolute;
  inset: 0 auto 0 0;
  width: var(--w);
  background: oklch(77% 0.115 190 / 0.34);
}

.restored .memory-bars > div::before {
  background: oklch(68% 0.18 344 / 0.34);
}

.memory-bars span {
  position: relative;
  z-index: 1;
  display: inline-block;
  padding: 9px 11px;
  color: var(--sb-soft);
  font: 800 10px/1 "SFMono-Regular", Menlo, monospace;
  text-transform: uppercase;
}

.state-foot {
  padding: 16px 18px;
  border-top: 1px solid var(--sb-line);
  color: var(--sb-soft);
  font-size: 13px;
}

.failure-axis {
  display: grid;
  justify-items: center;
  gap: 13px;
  text-align: center;
  font-family: "SFMono-Regular", Menlo, monospace;
  text-transform: uppercase;
}

.failure-axis span {
  color: var(--sb-muted);
  font-size: 10px;
  font-weight: 800;
}

.failure-axis i {
  width: 1px;
  height: 58px;
  background: var(--sb-pink);
}

.failure-axis strong {
  padding: 12px 15px;
  background: var(--sb-pink);
  color: var(--sb-bg-deep);
  font-size: 12px;
  transform: rotate(-1deg);
}

.inspector-wrap {
  height: 100%;
  display: grid;
  grid-template-columns: 0.34fr 0.66fr;
  grid-template-rows: 1fr auto;
  gap: 18px;
}

.session-rail,
.memory-inspector {
  border: 1px solid var(--sb-line);
  background: oklch(18% 0.042 272 / 0.9);
}

.rail-head {
  padding: 18px;
  border-bottom: 1px solid var(--sb-line);
}

.session {
  padding: 17px 18px;
  display: grid;
  gap: 7px;
  border-bottom: 1px solid var(--sb-line);
}

.session strong {
  font-size: 15px;
}

.session.active {
  border-left: 3px solid var(--sb-teal);
  background: oklch(77% 0.115 190 / 0.08);
}

.memory-inspector {
  display: grid;
  grid-template-rows: auto 1fr auto;
}

.inspector-head {
  padding: 18px;
  display: grid;
  grid-template-columns: 1fr 0.72fr;
  gap: 20px;
  align-items: center;
  border-bottom: 1px solid var(--sb-line);
}

.inspector-head > div:first-child {
  display: grid;
  gap: 7px;
}

.inspector-head strong {
  font-size: 17px;
}

.search-field {
  min-height: 38px;
  padding: 12px 14px;
  border: 1px solid oklch(77% 0.115 190 / 0.42);
  color: var(--sb-teal-soft);
  font: 800 12px/1 "SFMono-Regular", Menlo, monospace;
}

.memory-results {
  padding: 18px;
  display: grid;
  align-content: center;
  gap: 12px;
}

.memory-results article {
  padding: 17px;
  display: grid;
  gap: 9px;
  border-left: 3px solid var(--sb-teal);
  background: oklch(77% 0.115 190 / 0.06);
}

.memory-results article > div {
  display: flex;
  justify-content: space-between;
}

.memory-results em {
  color: var(--sb-teal-soft);
  font: 850 10px/1 "SFMono-Regular", Menlo, monospace;
  font-style: normal;
}

.memory-results strong {
  font-size: 16px;
}

.memory-results p {
  color: var(--sb-muted);
  font-size: 12px;
}

.memory-actions {
  padding: 14px 18px;
  display: flex;
  gap: 24px;
  justify-content: flex-end;
  border-top: 1px solid var(--sb-line);
  color: var(--sb-teal-soft);
}

.inspector-wrap footer {
  grid-column: 1 / 3;
  display: grid;
  grid-template-columns: auto 1fr auto;
  gap: 18px;
  align-items: center;
  padding-top: 14px;
  border-top: 1px solid var(--sb-line);
}

.inspector-wrap footer strong {
  color: var(--sb-yellow-soft);
  font-size: 14px;
  text-align: center;
}
</style>
