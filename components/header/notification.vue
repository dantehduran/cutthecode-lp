<script setup lang="ts">
import { Button } from "../ui/button";
const items = [
  { title: "Reducations", desc: "A platform for the education of the future" },
  {
    title: "Samsung x Skybox",
    desc: "Next-level inspiration platform for Gen Z",
  },
  { title: "SelektHuis", desc: "  Growth-driven platform for a market leader" },
  { title: "Jay-Jay Boske", desc: "Personal branding experience" },
];
</script>

<template>
  <div class="overflow-hidden relative z-0 box-border">
    <div
      class="overflow-hidden flex justify-start items-center text-sm leading-4 pl-4 pr-14 h-12"
    >
      <div
        class="pr-4 pl-4 md:pl-8 text-sm h-full text-zinc-200 items-center whitespace-pre flex font-extrabold"
      >
        <div class="mr-2 w-2 h-2 bg-red-500 rounded-full"></div>
        <div>Now Creating<br /></div>
      </div>
      <!--container-->
      <div class="w-full h-full items-center flex relative overflow-hidden">
        <div
          class="w-10 md:w-28 z-10 h-full absolute inset-y-0 left-0 bg-gradient-to-r from-background"
        ></div>
        <div
          class="w-10 md:w-28 z-10 h-full absolute inset-y-0 right-0 bg-gradient-to-l from-background"
        ></div>
        <div class="whitespace-nowrap telepromt flex max-w-fit gap-8">
          <div
            v-for="(item, index) in [...items, ...items]"
            :key="index"
            class="flex gap-2"
          >
            <div class="opacity-80">{{ item.title }}</div>
            <div class="opacity-40">
              {{ item.desc }}
            </div>
          </div>
        </div>
      </div>
      <div class="ml-0 md:ml-4 flex items-center bg-scroll w-12 min-w-[3rem]">
        <!--TODO: border color and gh color-->
        <Button variant="outline" class="rounded-full">EN</Button>
      </div>
    </div>
  </div>
</template>

<style>
@keyframes text-scroll {
  to {
    transform: translateX(calc(-50% - 1rem));
  }
}
.telepromt {
  animation: text-scroll 20s linear infinite;
}
</style>
