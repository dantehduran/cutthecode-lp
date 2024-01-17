<template>
  <div
    class="group relative w-[22rem] flex-shrink-0 flex flex-col gap-6 cursor-pointer"
  >
    <div
      class="relative aspect-[3/4] overflow-hidden max-w-[22rem] rounded-2xl"
    >
      <img
        :src="'/images' + img"
        :alt="client"
        class="object-cover group-hover:scale-105 transition duration-300"
      />
      <div
        class="absolute bottom-0 w-full flex justify-center items-start p-6 transition-all duration-300 ease-in-out transform translate-y-full group-hover:translate-y-0"
      >
        <div
          class="w-full bg-muted opacity-95 rounded-2xl p-6 flex flex-col gap-4 justify-start"
        >
          <div class="flex flex-col gap-2 justify-start items-start">
            <span class="text-muted-foreground opacity-95">Used Tools</span>
            <div class="flex flex-wrap gap-1">
              <div
                class="text-sm font-semibold rounded-full py-1 px-2 bg-background/95 text-foreground"
                v-for="tool in tools"
              >
                {{ tool }}
              </div>
            </div>
          </div>
          <div class="flex flex-col gap-1 justify-start items-start">
            <span class="text-muted-foreground opacity-95">
              Build to launch
            </span>
            <span class="text-foreground font-semibold">{{ buildTime }}</span>
          </div>
          <Button v-if="case" variant="default" size="sm">Show case</Button>
          <Button v-else variant="outline" size="sm">Visit website</Button>
        </div>
      </div>
    </div>
    <div class="flex flex-col gap-1">
      <h3 class="flex whitespace-normal text-balance text-2xl text-foreground">
        {{ desc }}
      </h3>
      <div class="opacity-60 font-semibold leading-[140%]">{{ client }}</div>
    </div>
    <div
      v-show="case"
      class="absolute top-0 -right-[1px] pl-4 pb-4 bg-muted rounded-bl-2xl flex justify-end items-start"
    >
      <div
        class="text-sm font-semibold rounded-full flex items-center py-1 px-2 bg-background text-foreground"
      >
        Case
      </div>
      <Curve class="absolute text-muted -left-3.5 top-0 rotate-90" />
      <Curve class="absolute text-muted -bottom-3.5 right-0 rotate-90" />
    </div>
  </div>
</template>
<script setup lang="ts">
import { Button } from "../ui/button";
defineProps({
  img: String,
  client: String,
  desc: String,
  case: Boolean,
  tools: Array<String>,
  buildTime: String,
});
</script>
<style>
.text-balance {
  text-wrap: balance;
}
</style>
