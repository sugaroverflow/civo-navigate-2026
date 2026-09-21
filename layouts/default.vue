<template>
  <div class="slidev-layout sb-layout">
    <div class="sb-grid-bg" aria-hidden="true"></div>

    <header class="sb-topbar" aria-hidden="true">
      <span>SPARKLE BUREAUCRACY / DEPT. OF AGENT SYSTEMS</span>
      <span>CIVO NAVIGATE 2026</span>
    </header>

    <main class="sb-stage">
      <slot />
    </main>

    <footer class="sb-global-footer" aria-hidden="true">
      my agent made these slides
    </footer>
  </div>
</template>
