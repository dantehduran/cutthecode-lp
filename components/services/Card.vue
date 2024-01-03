<template>
  <div
    class="group rounded-2xl w-full pr-6 py-8 pl-8 border-r border-r-primary/50"
  >
    <div class="flex flex-col gap-4">
      <div class="flex items-center gap-4 transform transition-all">
        <div class="w-16 scale-0 group-hover:scale-100 duration-200 ease-out">
          <img :src="'/images/' + icon" alt="" />
        </div>
        <h4
          class="text-4xl capitalize font-light -translate-x-20 group-hover:translate-x-0 duration-500 ease-out"
        >
          {{ title }}
        </h4>
      </div>
      <div class="text-opacity-60 leading-relaxed font-sans font-normal w-4/5">
        {{ description }}
      </div>
    </div>
  </div>
</template>
<script setup lang="ts">
defineProps({
  title: String,
  description: String,
  icon: String,
});
</script>
