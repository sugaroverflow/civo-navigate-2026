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
        :src="withBase('/assets/screenshots/civo/jer-crane-x-post-cover.jpg')"
        alt="Excerpt from Jer Crane's original X post about the production incident"
      />
      <figcaption>Jer Crane · @lifeof_jer · original post</figcaption>
    </figure>

    <div class="incident-admission">
      <span class="incident-source">THE AGENT'S ADMISSION</span>
      <div class="incident-quote">“I violated every principle I was given.”</div>
      <div class="incident-blast-radius">
        <span>credential escaped staging</span>
        <i></i>
        <span>account-wide delete</span>
        <i></i>
        <span>database + backups</span>
      </div>
      <a href="https://x.com/lifeof_jer/status/2048103471019434248">source: x.com/lifeof_jer</a>
    </div>
  </div>
</template>
