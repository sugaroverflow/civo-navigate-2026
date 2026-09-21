<script setup>
const withBase = (src) => {
  if (!src.startsWith("/")) return src;
  return `${import.meta.env.BASE_URL}${src.slice(1)}`;
};
</script>

<template>
  <div class="incident-post-layout">
    <figure class="incident-post-shot">
      <img
        :src="withBase('/assets/screenshots/civo/jer-crane-long.webp')"
        alt="Jer Crane's long-form post describing the production database incident"
      />
      <figcaption>Jer Crane · nine seconds</figcaption>
    </figure>

    <div class="incident-admission">
      <span class="incident-source">THE AGENT'S ADMISSION</span>
      <div class="incident-quote">“I violated every principle I was given.”</div>
      <a href="https://x.com/lifeof_jer/status/2048103471019434248">source: x.com/lifeof_jer</a>
    </div>
  </div>
</template>
