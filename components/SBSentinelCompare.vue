<template>
  <div class="sentinel-wrap">
    <div class="compare-grid">
      <section class="system system-bubbles">
        <header><span>FEBRUARY</span><strong>BUBBLES / SELF-HOSTED</strong></header>
        <div class="system-body">
          <div class="machine-label">£6 VPS</div>
          <div class="runtime-box">
            <span>OpenClaw</span>
            <strong>Bubbles</strong>
            <small>memory · tools · credentials</small>
          </div>
          <div class="outbound direct"><i></i><span>internet</span></div>
          <div class="system-note">No independent policy gate</div>
        </div>
      </section>

      <section class="system system-muse">
        <header><span>SEPTEMBER</span><strong>MUSE / META CLOUD</strong></header>
        <div class="system-body">
          <div class="machine-label">MUSE SECURE VM</div>
          <div class="muse-stack">
            <div class="runtime-box">
              <span>agent</span>
              <strong>Muse</strong>
              <small>memory · browser · tools</small>
            </div>
            <div class="sentinel-box">
              <span>policy agent</span>
              <strong>Sentinel</strong>
              <small>system-level separation</small>
            </div>
          </div>
          <div class="outbound gated"><i></i><span>approved internet</span></div>
          <div class="audit-strip">audit trail · planned actions · approval</div>
        </div>
      </section>
    </div>

    <footer>
      <span>same runtime pattern</span>
      <strong>different answer to “who holds the box?”</strong>
      <span>source: Meta · 08 SEP 2026</span>
    </footer>
  </div>
</template>

<style scoped>
.sentinel-wrap {
  height: 100%;
  display: grid;
  grid-template-rows: 1fr auto;
  gap: 22px;
}

.compare-grid {
  display: grid;
  grid-template-columns: 0.86fr 1.14fr;
  gap: 28px;
  min-height: 0;
}

.system {
  border: 1px solid var(--sb-line);
  background: oklch(18% 0.042 272 / 0.9);
  box-shadow: 0 24px 64px oklch(5% 0.025 270 / 0.24);
}

.system > header {
  min-height: 54px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 16px;
  padding: 0 18px;
  border-bottom: 1px solid var(--sb-line);
  font-family: "SFMono-Regular", Menlo, monospace;
}

.system > header span {
  color: var(--sb-muted);
  font-size: 11px;
  font-weight: 800;
}

.system > header strong {
  font-size: 12px;
}

.system-bubbles {
  border-color: oklch(68% 0.18 344 / 0.35);
  transform: translateY(28px) rotate(-0.4deg);
}

.system-muse {
  border-color: oklch(77% 0.115 190 / 0.5);
  transform: rotate(0.35deg);
}

.system-body {
  position: relative;
  min-height: 410px;
  display: grid;
  align-content: center;
  gap: 22px;
  padding: 34px;
  overflow: hidden;
}

.machine-label {
  position: absolute;
  top: 14px;
  left: 16px;
  color: var(--sb-muted);
  font: 800 10px/1 "SFMono-Regular", Menlo, monospace;
}

.runtime-box,
.sentinel-box {
  min-width: 0;
  min-height: 150px;
  display: grid;
  place-content: center;
  gap: 8px;
  padding: 24px;
  border: 1px solid oklch(68% 0.18 344 / 0.5);
  background: oklch(22% 0.05 272 / 0.92);
  text-align: center;
}

.runtime-box span,
.sentinel-box span {
  color: var(--sb-muted);
  font: 800 10px/1 "SFMono-Regular", Menlo, monospace;
  text-transform: uppercase;
}

.runtime-box strong,
.sentinel-box strong {
  font-size: 28px;
}

.runtime-box small,
.sentinel-box small {
  color: var(--sb-soft);
  font: 700 11px/1.35 "SFMono-Regular", Menlo, monospace;
}

.muse-stack {
  display: grid;
  grid-template-columns: 1fr 0.82fr;
  gap: 16px;
}

.system-muse .runtime-box {
  border-color: oklch(77% 0.115 190 / 0.48);
}

.sentinel-box {
  border-color: oklch(87% 0.13 92 / 0.68);
  background: oklch(87% 0.13 92 / 0.08);
}

.sentinel-box strong {
  color: var(--sb-yellow-soft);
}

.outbound {
  display: grid;
  grid-template-columns: 1fr auto;
  gap: 12px;
  align-items: center;
  color: var(--sb-soft);
  font: 800 11px/1 "SFMono-Regular", Menlo, monospace;
  text-transform: uppercase;
}

.outbound i {
  height: 1px;
  background: var(--sb-pink);
}

.outbound.gated i {
  background: linear-gradient(90deg, var(--sb-yellow), var(--sb-teal));
}

.system-note,
.audit-strip {
  padding: 12px 14px;
  border-left: 3px solid var(--sb-pink);
  background: oklch(68% 0.18 344 / 0.08);
  color: var(--sb-pink-soft);
  font: 800 12px/1.35 "SFMono-Regular", Menlo, monospace;
}

.audit-strip {
  border-left-color: var(--sb-teal);
  background: oklch(77% 0.115 190 / 0.08);
  color: var(--sb-teal-soft);
}

footer {
  display: grid;
  grid-template-columns: auto 1fr auto;
  gap: 22px;
  align-items: center;
  padding-top: 18px;
  border-top: 1px solid var(--sb-line);
  font-family: "SFMono-Regular", Menlo, monospace;
  text-transform: uppercase;
}

footer span {
  color: var(--sb-muted);
  font-size: 10px;
  font-weight: 800;
}

footer strong {
  color: var(--sb-yellow-soft);
  font-size: 16px;
  text-align: center;
}
</style>
