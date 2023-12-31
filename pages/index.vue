<template>
  <div
    class="leading-relaxed md:leading-none antialiased bg-background font-sans min-h-full dark mt-2"
  >
    <HeaderNotification />
    <HeaderNav />
    <main class="z-0 relative bg-background">
      <HeaderHero />
      <ServicesContainer />
    </main>
  </div>
</template>
<script setup lang="ts">
useHead({
  title: "No-Code Agency & Webflow Partner for Ambitious Brands",
  meta: [{ name: "description", content: "No-Code landing page" }],
  bodyAttrs: {
    class: "dark",
  },
});
</script>
