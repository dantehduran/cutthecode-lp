<template>
  <div class="flex justify-end">
    <!--group button-->
    <div class="flex gap-4 justify-center items-center">
      <button
        v-for="(link, index) in links"
        :key="index"
        class="group relative h-8 pl-5 pr-2 rounded-md flex justify-center items-center hover:bg-gradient-to-tl hover:from-[rgba(214,163,228,0.16)] hover:to-[rgba(214,163,228,0)] transition-all duration-500 ease-in"
      >
        <Dot
          class="scale-0 group-hover:scale-100 transition-all ease-out duration-300 absolute top-1/2 left-2.5 transform -translate-x-1/2 -translate-y-1/3"
        />
        <span class="capitalize">{{ link.name }}</span>
      </button>
    </div>
  </div>
</template>
<script setup lang="ts">
const links = [
  { name: "no-code", to: "/" },
  { name: "projects", to: "/projects" },
  { name: "about us", to: "/aboutus" },
  { name: "contact", to: "/contact" },
];
</script>
