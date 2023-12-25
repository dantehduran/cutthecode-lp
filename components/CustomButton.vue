<template>
  <button class="flex z-10 items-center relative group transition-all">
    <div
      class="w-12 h-12 flex justify-center items-center rounded-2xl scale-100 group-hover:scale-0 duration-300 transform ease-in-out"
      v-bind="$attrs"
    >
      <div class="w-5 h-5 flex justify-center items-center">
        <slot name="icon"></slot>
      </div>
    </div>
    <div
      class="z-10 h-12 rounded-2xl pb-0.5 px-4 flex justify-center items-center whitespace-pre text-lg font-semibold group-hover:-translate-x-12 duration-300 transform ease-in-out"
      v-bind="$attrs"
    >
      <slot></slot>
    </div>
    <div
      class="w-12 h-12 flex justify-center items-center rounded-2xl absolute right-0 scale-0 group-hover:scale-100 duration-300 transform ease-in-out"
      v-bind="$attrs"
    >
      <div class="w-5 h-5 flex justify-center items-center">
        <slot name="icon"></slot>
      </div>
    </div>
  </button>
</template>
<script setup lang="ts">
defineOptions({ inheritAttrs: false });
</script>
