<template>
  <div class="w-80 flex-shrink-0 flex flex-col gap-6 cursor-pointer">
    <div class="w-full aspect-[3/4] rounded-2xl">
      <img
        :src="'/images' + img"
        :alt="client"
        class="object-cover aspect-[3/4] rounded-2xl"
      />
    </div>
    <div class="flex flex-col gap-1">
      <h3 class="flex whitespace-normal text-balance text-2xl text-foreground">
        {{ desc }}
      </h3>
      <div class="opacity-60 font-semibold leading-[140%]">{{ client }}</div>
    </div>
  </div>
</template>
<script setup lang="ts">
defineProps({
  img: String,
  client: String,
  desc: String,
  case: Boolean,
});
</script>
<style>
.text-balance {
  text-wrap: balance;
}
</style>
