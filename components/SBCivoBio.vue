<template>
  <div class="bio-grid">
    <div class="bio-portrait-wrap">
      <SBPublicImage
        class="bio-portrait"
        src="/assets/screenshots/headshot-khalidfatima.png"
        alt="Fatima Sarah Khalid"
      />
      <div class="bio-coordinate">OPEN SOURCE · CIVIC TECH · AGENT SYSTEMS</div>
    </div>

    <div class="bio-copy">
      <div class="bio-kicker">AI ENGINEER &amp; CIVIC HACKER</div>
      <h2>Fatima Sarah Khalid</h2>
      <p class="bio-role">Senior Developer Advocate, GitLab</p>
      <p class="bio-thesis">Prototyping emerging technology, teaching it, and testing what happens when it meets real systems.</p>

      <div class="bio-cards">
        <article>
          <span>NOW</span>
          <strong>AI/ML R&amp;D · workshops · demos · agentic workflows</strong>
        </article>
        <article>
          <span>FIELDWORK</span>
          <strong>Newspeak House · Campaign Factory · ClawClub</strong>
        </article>
        <article>
          <span>ROOTS</span>
          <strong>Drupal Layout Builder · Diversity &amp; Inclusion · civic tech</strong>
        </article>
      </div>

      <div class="bio-stage-line">
        <strong>International keynote speaker</strong>
        <span>All Things Open · Open Source Summit NA</span>
      </div>

      <div class="bio-footer">
        <span>@sugaroverflow</span>
        <span>Monday Merge · The Developer Show</span>
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
.bio-cards span {
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

.bio-thesis {
  max-width: 720px;
  color: var(--sb-soft);
  font-size: 19px;
  line-height: 1.25;
  font-weight: 620;
}

.bio-cards {
  display: grid;
  gap: 8px;
  margin-top: 4px;
}

.bio-cards article {
  display: grid;
  grid-template-columns: 118px 1fr;
  gap: 18px;
  align-items: center;
  min-height: 66px;
  padding: 12px 16px;
  border: 1px solid var(--sb-line);
  background: oklch(94% 0.018 275 / 0.035);
}

.bio-cards article:nth-child(2) {
  background: oklch(77% 0.115 190 / 0.065);
}

.bio-cards span {
  color: var(--sb-muted);
  font-size: 11px;
  font-weight: 800;
}

.bio-cards strong {
  color: var(--sb-ink);
  font-size: 17px;
  font-weight: 720;
}

.bio-stage-line {
  display: grid;
  grid-template-columns: auto 1fr;
  gap: 14px;
  align-items: center;
  padding-top: 4px;
}

.bio-stage-line strong {
  color: var(--sb-yellow-soft);
  font-size: 15px;
}

.bio-stage-line span {
  color: var(--sb-soft);
  font-size: 14px;
}

.bio-footer {
  display: flex;
  justify-content: space-between;
  gap: 28px;
  color: var(--sb-soft);
  font-size: 12px;
  font-weight: 750;
}
</style>
