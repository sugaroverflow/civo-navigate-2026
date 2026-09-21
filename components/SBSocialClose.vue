<script setup>
const withBase = (src) => {
  if (!src.startsWith("/")) return src;
  return `${import.meta.env.BASE_URL}${src.slice(1)}`;
};
</script>

<template>
  <div class="social-close">
    <section class="social-thanks">
      <h2>THANK YOU!</h2>
      <div class="social-copy">
        <p class="social-handle">@sugaroverflow</p>
        <p class="social-caption">find me all over the internet as @sugaroverflow!</p>
      </div>
    </section>

    <section class="social-lab">
      <div class="social-lab-rule" aria-hidden="true"></div>
      <p>A network using emerging technology — AI agents, factories — to prototype more optimistic futures.</p>
      <div class="social-qr-frame">
        <img :src="withBase('/assets/sparkle-bureaucracy-qr.svg')" alt="QR code for sparklebureaucracy.org" />
      </div>
      <a class="social-url" href="https://www.sparklebureaucracy.org/">sparklebureaucracy.org</a>
    </section>
  </div>
</template>
