<template>
  <div class="bio-grid">
    <div class="bio-portrait-wrap">
      <SBPublicImage
        class="bio-portrait"
        src="/assets/screenshots/headshot-khalidfatima.png"
        alt="Fatima Sarah Khalid"
      />
      <div class="bio-coordinate">RAN CLAWCON LONDON · RUNS CLAWCLUB</div>
    </div>

    <div class="bio-copy">
      <div class="bio-kicker">FIELD REPORTER / OPERATOR</div>
      <h2>Fatima Sarah Khalid</h2>
      <p class="bio-role">Senior Developer Advocate, GitLab</p>

      <div class="bio-ledger">
        <div><span>work</span><strong>AI · DevSecOps · open source</strong></div>
        <div><span>fellowship</span><strong>Newspeak House — London's College of Political Technology</strong></div>
        <div><span>community</span><strong>ClawClub · ClawCon London</strong></div>
        <div><span>shows</span><strong>Monday Merge · The Developer Show</strong></div>
        <div><span>seen at</span><strong>All Things Open 2024 · Open Source Summit NA 2023</strong></div>
      </div>

      <div class="bio-footer">
        <span>@sugaroverflow</span>
        <span>AI · DevSecOps · open source</span>
      </div>
    </div>
  </div>
</template>

<style scoped>
.bio-grid {
  height: 100%;
  display: grid;
  grid-template-columns: 0.72fr 1.28fr;
  gap: 58px;
  align-items: center;
}

.bio-portrait-wrap {
  position: relative;
  width: min(100%, 390px);
  justify-self: end;
  transform: rotate(-1.2deg);
}

.bio-portrait {
  display: block;
  width: 100%;
  aspect-ratio: 4 / 5;
  object-fit: cover;
  object-position: 50% 30%;
  filter: saturate(0.88) contrast(1.05);
  border: 1px solid oklch(77% 0.115 190 / 0.55);
  box-shadow: 0 28px 70px oklch(5% 0.025 270 / 0.34);
}

.bio-coordinate {
  position: absolute;
  right: -24px;
  bottom: 28px;
  padding: 10px 14px;
  background: oklch(87% 0.13 92);
  color: oklch(14% 0.045 272);
  font: 850 12px/1 "SFMono-Regular", Menlo, monospace;
  letter-spacing: 0.04em;
}

.bio-copy {
  display: grid;
  gap: 14px;
  align-content: center;
  max-width: 760px;
}

.bio-kicker,
.bio-footer,
.bio-ledger span {
  font-family: "SFMono-Regular", Menlo, monospace;
  text-transform: uppercase;
}

.bio-kicker {
  color: var(--sb-teal-soft);
  font-size: 13px;
  font-weight: 850;
}

.bio-copy h2 {
  font-size: 58px;
  letter-spacing: -0.04em;
}

.bio-role {
  color: var(--sb-pink-soft);
  font-size: 25px;
  font-weight: 750;
}

.bio-ledger {
  margin-top: 8px;
  border-top: 1px solid var(--sb-line);
}

.bio-ledger > div {
  display: grid;
  grid-template-columns: 112px 1fr;
  gap: 22px;
  padding: 11px 0;
  border-bottom: 1px solid var(--sb-line);
}

.bio-ledger span {
  color: var(--sb-muted);
  font-size: 11px;
  font-weight: 800;
}

.bio-ledger strong {
  color: var(--sb-ink);
  font-size: 16.5px;
  font-weight: 720;
}

.bio-footer {
  display: flex;
  gap: 28px;
  color: var(--sb-soft);
  font-size: 12px;
  font-weight: 750;
}
</style>
