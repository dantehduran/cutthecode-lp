<template>
  <div
    class="absolute bottom-0 right-0 max-h-[28rem] max-w-2xl h-[27vw] w-[38vw]"
  >
    <div class="z-20 max-w-2xl flex flex-col-reverse">
      <div class="relative w-80 h-28 bg-background self-end">
        <Curve
          class="absolute text-background -left-3.5 bottom-0.5 rotate-180"
        />
        <Curve class="absolute text-background -top-3.5 right-0 rotate-180" />
        <Curve class="absolute text-background top-0 -left-3.5 rotate-90" />
      </div>
      <div class="relative w-80 h-28 bg-background self-start rounded-l-2xl">
        <Curve class="absolute text-background top-0 -right-3.5 rotate-0" />
        <Curve
          class="absolute text-background bottom-0 -right-3.5 -rotate-90"
        />
      </div>
      <div class="relative w-80 h-28 bg-background self-center rounded-r-2xl">
        <Curve
          class="absolute text-background -bottom-0.5 -left-3.5 rotate-180"
        />
        <Curve class="absolute text-background top-0 -left-3.5 rotate-90" />
      </div>
      <div
        class="relative w-16 h-16 bg-background rounded-t-2xl rounded-bl-2xl ml-14"
      >
        <Curve
          class="absolute text-background -bottom-0.5 -right-3.5 -rotate-90"
        />
      </div>
    </div>
  </div>
</template>
<script setup lang="ts"></script>
