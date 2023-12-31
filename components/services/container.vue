<template>
  <section class="flex flex-col px-5 w-full mx-auto relative">
    <div class="h-36 w-full absolute top-0 right-5">
      <div
        class="w-2/5 h-full absolute top-0 right-0 rounded-b-2xl bg-muted z-40"
      >
        <Curve class="text-muted top-0 -left-4 rotate-90" />
      </div>
    </div>
    <div class="w-full px-16">
      <div class="relative">
        <div class="absolute -top-10 left-6">
          <div
            class="py-3 px-4 whitespace-nowrap rounded-t-2xl bg-background flex items-center overflow-hidden gap-2"
          >
            <Dot class="h-2 w-2 overflow-hidden" />
            <h4 class="font-bold">Services</h4>
          </div>
          <Curve
            class="text-background absolute bottom-0 -right-4 -rotate-90"
          />
          <Curve
            class="text-background absolute bottom-0 -left-3.5 rotate-180"
          />
        </div>
        <div class="py-24">
          <div class="w-3/5 max-w-2xl">
            <h3 class="text-5xl">
              We create without the need for coding to give ambitious brands the
              upper hand
            </h3>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
