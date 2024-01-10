<template>
  <section class="px-5 mx-auto w-full">
    <div
      class="flex bg-accent rounded-2xl relative w-full text-accent-foreground"
    >
      <div class="w-full px-16 md:pl-40 py-24 mx-auto">
        <div class="max-w-xl flex flex-col gap-4">
          <div class="flex gap-2 items-center">
            <Dot class="w-2 h-2 bg-rose-500" />
            <h4 class="font-bold">Our Vision</h4>
          </div>
          <h2 class="font-light text-6xl">The no-code revolution</h2>
          <p class="opacity-80 text-xl font-normal w-full max-w-[28rem]">
            The digital world is changing. Brands need to be fast, creative, and
            flexible. That’s where no-code comes in: a cutting-edge movement
            which allows you to design and create digital products without
            needing programming know-how. Meaning brands can move faster, build
            smarter, and scale more, by coding less.
          </p>
          <div class="flex items-center mt-2">
            <CustomButton class="bg-primary text-primary-foreground"
              >More About No-Code<template #icon
                ><svg
                  height="100%"
                  viewBox="0 0 24 23"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M15.7196 11.9163C13.8735 11.9163 12.3279 13.3863 12.3279 15.2342V22.5H11.641V15.2342C11.641 13.3863 10.0954 11.9163 8.20639 11.9163H0.822021V11.2443H8.20639C10.0954 11.2023 11.641 9.73237 11.5981 7.88442V0.660645H12.3279V7.88442C12.3279 9.73237 13.8735 11.2023 15.7196 11.2023H23.1469V11.9163H15.7196Z"
                    fill="currentColor"
                  ></path></svg></template
            ></CustomButton>
          </div>
        </div>
      </div>
      <VisionTools />
    </div>
  </section>
</template>
