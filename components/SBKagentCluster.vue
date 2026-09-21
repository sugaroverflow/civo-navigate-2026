<template>
  <div class="cluster-wrap">
    <section class="agent-plane">
      <div class="plane-label">AGENTS AS CUSTOM RESOURCES</div>
      <div class="agents">
        <div><span>CR</span><strong>triage-agent</strong><small>observe</small></div>
        <i></i>
        <div><span>CR</span><strong>diagnose-agent</strong><small>delegate / A2A</small></div>
        <i></i>
        <div><span>CR</span><strong>repair-agent</strong><small>approve-to-apply</small></div>
      </div>
    </section>

    <section class="cluster-plane">
      <div class="cluster-head">
        <span>KUBERNETES CLUSTER / DELIBERATELY BROKEN</span>
        <strong>5 / 5 FIXED</strong>
      </div>
      <div class="fault-grid">
        <div v-for="fault in faults" :key="fault.name" class="fault">
          <span>{{ fault.code }}</span>
          <strong>{{ fault.name }}</strong>
          <small>{{ fault.fix }}</small>
          <em>FIXED</em>
        </div>
      </div>
    </section>

    <footer>
      <span>technical result: capable</span>
      <strong>operator verdict: not on a client cluster — not even read-only</strong>
    </footer>
  </div>
</template>

<script setup>
const faults = [
  { code: "F-01", name: "OOMKilled", fix: "resource limits" },
  { code: "F-02", name: "CrashLoopBackOff", fix: "runtime config" },
  { code: "F-03", name: "bad image tag", fix: "deployment image" },
  { code: "F-04", name: "probe → 404", fix: "readiness path" },
  { code: "F-05", name: "Redis → 0", fix: "restore replicas" },
];
</script>

<style scoped>
.cluster-wrap {
  height: 100%;
  display: grid;
  grid-template-rows: auto 1fr auto;
  gap: 18px;
}

.agent-plane {
  display: grid;
  grid-template-columns: 190px 1fr;
  gap: 20px;
  align-items: center;
  padding: 14px 18px;
  border: 1px solid oklch(77% 0.115 190 / 0.4);
  background: oklch(77% 0.115 190 / 0.06);
}

.plane-label,
.cluster-head,
.fault span,
.fault em,
footer {
  font-family: "SFMono-Regular", Menlo, monospace;
  text-transform: uppercase;
}

.plane-label {
  color: var(--sb-teal-soft);
  font-size: 10px;
  font-weight: 850;
}

.agents {
  display: grid;
  grid-template-columns: 1fr 38px 1fr 38px 1fr;
  align-items: center;
}

.agents > div {
  min-height: 58px;
  padding: 11px 13px;
  display: grid;
  grid-template-columns: auto 1fr;
  column-gap: 10px;
  align-items: center;
  border-left: 2px solid var(--sb-teal);
  background: oklch(94% 0.018 275 / 0.035);
}

.agents span {
  grid-row: 1 / 3;
  color: var(--sb-teal-soft);
  font: 850 9px/1 "SFMono-Regular", Menlo, monospace;
}

.agents strong {
  font-size: 14px;
}

.agents small {
  color: var(--sb-muted);
  font-size: 10px;
}

.agents i {
  height: 1px;
  background: var(--sb-teal);
}

.cluster-plane {
  min-height: 0;
  border: 1px solid var(--sb-line);
  background: oklch(18% 0.042 272 / 0.88);
}

.cluster-head {
  height: 45px;
  padding: 0 16px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  border-bottom: 1px solid var(--sb-line);
  color: var(--sb-muted);
  font-size: 10px;
  font-weight: 850;
}

.cluster-head strong {
  color: var(--sb-teal-soft);
}

.fault-grid {
  height: calc(100% - 45px);
  display: grid;
  grid-template-columns: repeat(5, 1fr);
}

.fault {
  position: relative;
  padding: 22px 16px;
  display: grid;
  align-content: center;
  gap: 12px;
  border-right: 1px solid var(--sb-line);
}

.fault:nth-child(odd) {
  background: oklch(94% 0.018 275 / 0.025);
}

.fault span {
  color: var(--sb-pink-soft);
  font-size: 9px;
  font-weight: 850;
}

.fault strong {
  font-size: 19px;
  line-height: 1.05;
}

.fault small {
  color: var(--sb-soft);
  font-size: 12px;
}

.fault em {
  position: absolute;
  right: 10px;
  bottom: 10px;
  color: var(--sb-teal-soft);
  font-size: 9px;
  font-style: normal;
  font-weight: 850;
}

footer {
  display: grid;
  grid-template-columns: auto 1fr;
  gap: 20px;
  align-items: center;
  padding-top: 15px;
  border-top: 1px solid var(--sb-line);
  color: var(--sb-muted);
  font-size: 10px;
  font-weight: 850;
}

footer strong {
  color: var(--sb-yellow-soft);
  font-size: 14px;
  text-align: right;
}
</style>
