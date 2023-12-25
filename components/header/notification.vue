<script setup lang="ts">
import { Button } from "../ui/button";
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
        <div class="whitespace-nowrap telepromt flex w-full gap-8">
          <div class="flex gap-2">
            <div class="opacity-80">primer anuncio</div>
            <div class="opacity-40">description 1 ...</div>
          </div>
          <div class="flex gap-2">
            <div class="opacity-80">segundo anuncio</div>
            <div class="opacity-40">description 2 ...</div>
          </div>
          <div class="flex gap-2">
            <div class="opacity-80">tercer anuncio</div>
            <div class="opacity-40">description 3 ...</div>
          </div>
          <div class="flex gap-2">
            <div class="opacity-80">cuarto anuncio</div>
            <div class="opacity-40">description 4 ...</div>
          </div>
        </div>
      </div>
      <div class="ml-0 md:ml-4 flex items-center bg-scroll w-12 min-w-[3rem]">
        <!--FIX: border color and gh color-->
        <Button variant="outline" class="rounded-full">EN</Button>
      </div>
    </div>
  </div>
</template>

<style>
@keyframes text-scroll {
  0% {
    transform: translateX(100%);
  }
  100% {
    transform: translateX(-100%);
  }
}
.telepromt {
  animation: text-scroll 20s linear infinite;
}
</style>
