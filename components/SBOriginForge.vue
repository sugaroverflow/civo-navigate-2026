<template>
  <div class="origin-wrap">
    <section class="branch-field">
      <div class="branch-head">
        <span>ORIGIN / AGENT FORGE</span>
        <strong>5 agents · 1 repository</strong>
      </div>
      <div class="branch-map">
        <div class="main-line"><span>main</span></div>
        <div v-for="(branch, index) in branches" :key="branch.name" class="branch-row">
          <i :style="{ '--offset': `${index * 16}px` }"></i>
          <span class="agent-id">{{ branch.agent }}</span>
          <strong>{{ branch.name }}</strong>
          <em>{{ branch.state }}</em>
        </div>
      </div>
    </section>

    <section class="tour-panel">
      <div class="tour-head">
        <span>CODE TOUR</span>
        <strong>PR #184</strong>
      </div>
      <ol>
        <li><span>01</span><div><strong>routing</strong><small>3 files · request flow</small></div></li>
        <li><span>02</span><div><strong>identity</strong><small>5 files · actor metadata</small></div></li>
        <li><span>03</span><div><strong>verification</strong><small>7 files · tests and checks</small></div></li>
      </ol>
      <div class="tour-chat">Ask the implementation instead of scrolling the diff.</div>
    </section>

    <div class="origin-footer">
      <span>native repo: source of truth</span>
      <span>mirrored repo: a window onto GitHub</span>
    </div>
  </div>
</template>

<script setup>
const branches = [
  { agent: "A-01", name: "spec/identity", state: "PR" },
  { agent: "A-02", name: "build/audit-log", state: "PR" },
  { agent: "A-03", name: "test/forge-sync", state: "COMMIT" },
  { agent: "A-04", name: "fix/reviewer-map", state: "PR" },
  { agent: "A-05", name: "verify/metadata", state: "COMMIT" },
];
</script>

<style scoped>
.origin-wrap {
  height: 100%;
  display: grid;
  grid-template-columns: 1.16fr 0.84fr;
  grid-template-rows: 1fr auto;
  gap: 22px;
}

.branch-field,
.tour-panel {
  border: 1px solid var(--sb-line);
  background: oklch(18% 0.042 272 / 0.88);
  min-height: 0;
}

.branch-head,
.tour-head {
  min-height: 48px;
  padding: 0 16px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  border-bottom: 1px solid var(--sb-line);
  font-family: "SFMono-Regular", Menlo, monospace;
}

.branch-head span,
.tour-head span {
  color: var(--sb-muted);
  font-size: 10px;
  font-weight: 850;
}

.branch-head strong,
.tour-head strong {
  color: var(--sb-teal-soft);
  font-size: 12px;
}

.branch-map {
  padding: 24px;
  display: grid;
  gap: 10px;
}

.main-line {
  margin-left: 62px;
  height: 28px;
  border-left: 2px solid var(--sb-soft);
  color: var(--sb-soft);
  font: 800 10px/1 "SFMono-Regular", Menlo, monospace;
}

.main-line span {
  margin-left: 10px;
}

.branch-row {
  min-height: 54px;
  display: grid;
  grid-template-columns: 48px 58px 1fr auto;
  gap: 12px;
  align-items: center;
  padding: 0 14px;
  background: oklch(94% 0.018 275 / 0.035);
}

.branch-row i {
  width: calc(26px + var(--offset));
  height: 18px;
  border-top: 2px solid var(--sb-pink);
  border-left: 2px solid var(--sb-pink);
  transform: translateY(8px);
}

.agent-id,
.branch-row em {
  font: 800 10px/1 "SFMono-Regular", Menlo, monospace;
  font-style: normal;
}

.agent-id {
  color: var(--sb-pink-soft);
}

.branch-row strong {
  font-size: 15px;
}

.branch-row em {
  color: var(--sb-yellow-soft);
}

.tour-panel {
  transform: translateY(20px) rotate(0.35deg);
}

.tour-panel ol {
  list-style: none;
  margin: 0;
  padding: 20px;
  display: grid;
  gap: 10px;
}

.tour-panel li {
  display: grid;
  grid-template-columns: 36px 1fr;
  gap: 12px;
  padding: 13px;
  border-left: 2px solid var(--sb-teal);
  background: oklch(77% 0.115 190 / 0.06);
}

.tour-panel li > span {
  color: var(--sb-teal-soft);
  font: 850 11px/1 "SFMono-Regular", Menlo, monospace;
}

.tour-panel li div {
  display: grid;
  gap: 5px;
}

.tour-panel li strong {
  font-size: 16px;
}

.tour-panel li small {
  color: var(--sb-muted);
  font-size: 12px;
}

.tour-chat {
  margin: 0 20px 20px;
  padding: 16px;
  border: 1px solid oklch(87% 0.13 92 / 0.36);
  color: var(--sb-yellow-soft);
  font-size: 15px;
  line-height: 1.35;
}

.origin-footer {
  grid-column: 1 / 3;
  display: grid;
  grid-template-columns: 1fr 1fr;
  border-top: 1px solid var(--sb-line);
}

.origin-footer span {
  padding: 14px 18px;
  color: var(--sb-soft);
  font: 800 11px/1 "SFMono-Regular", Menlo, monospace;
  text-transform: uppercase;
}

.origin-footer span:last-child {
  border-left: 1px solid var(--sb-line);
  color: var(--sb-yellow-soft);
}
</style>
