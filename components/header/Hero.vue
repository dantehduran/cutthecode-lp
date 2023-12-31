<template>
  <section>
    <div class="px-5 mx-auto w-full">
      <div
        class="bg-muted relative overflow-hidden rounded-t-3xl rounded-bl-3xl"
      >
        <div class="px-8 md:w-full md:px-16 pb-2 sm:pb-20">
          <div class="mx-auto w-full max-w-[96rem]">
            <div class="px-6 md:px-8 pt-28 md:pt-36 flex flex-col gap-4">
              <div class="flex gap-4 justify-start items-center">
                <Dot class="text-primary scale-150" />
                <span class="font-extrabold text-lg leading-5 capitalize">
                  leading No-Code & webflow agency
                </span>
              </div>
              <h2 class="text-8xl tracking-wide">
                We enable rapid growth through digital creation
              </h2>
              <div class="flex justify-between items-end py-4 w-full md:w-5/6">
                <div class="opacity-80 w-1/2 text-lg font-semibold">
                  Cut the Code is a leading no-code agency & Webflow Partner
                  based in Amsterdam, The Netherlands. We push our clients
                  forward into tomorrow - and fast - by creating the next
                  generation of web experiences.
                </div>
                <div class="w-1/4 flex z-20 gap-4 justify-center items-center">
                  <div class="min-w-fit">
                    <img src="/images/logos/partner-wf.svg" alt="partner wf" />
                  </div>
                  <div class="flex justify-center items-center">
                    <CustomButton class="bg-white text-background">
                      Learn more
                      <template #icon>
                        <svg
                          height="100%"
                          viewBox="0 0 15 18"
                          fill="none"
                          xmlns="http://www.w3.org/2000/svg"
                        >
                          <path
                            d="M8.46009 0.277253L8.20565 14.8126L9.03122 14.8258C9.20577 13.8891 9.7077 13.0326 10.4588 12.3896L13.3614 9.77656L14.525 10.8997L7.29573 17.4076L0.332226 10.6856L1.53713 9.60089L4.25203 12.2216C5.02837 12.895 5.52057 13.8051 5.63975 14.7874L6.50104 14.8014L6.77329 0.25L8.46009 0.277253Z"
                            fill="currentColor"
                          ></path>
                        </svg>
                      </template>
                    </CustomButton>
                  </div>
                </div>
              </div>
            </div>
            <div class="-mt-12 w-full relative">
              <div class="w-11/12 h-16 bg-muted absolute top-0 rounded-br-2xl">
                <Curve class="top-0 -right-4 text-muted" />
                <Curve class="left-0 -bottom-4 text-muted" />
              </div>
              <div
                class="w-20 h-3/6 bg-muted absolute left-0 bottom-0 rounded-tr-2xl"
              >
                <Curve class="left-0 -top-4 text-muted -rotate-90" />
                <Curve class="bottom-0 -right-4 text-muted -rotate-90" />
              </div>
              <div
                class="w-1/5 h-28 bg-muted absolute bottom-0 right-0 rounded-tl-2xl"
              >
                <Curve class="right-0 -top-4 text-muted rotate-180" />
                <Curve class="bottom-0 -left-4 text-muted rotate-180" />
              </div>
              <div
                class="w-full h-[500px] bg-cover bg-center rounded-t-2xl"
                style="
                  background-image: url(&quot;/images/home-header.webp&quot;);
                "
              ></div>
            </div>
            <div class="w-full my-8">
              <div class="flex justify-between items-center gap-4">
                <img
                  class="w-[10vw] max-w-[10rem] max-h-16 object-contain"
                  v-for="logo in logoList"
                  :src="logo.name"
                  :alt="logo.alt"
                />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script setup lang="ts">
const logoList = [
  { name: "/images/logos/samsung.svg", alt: "samsung logo" },
  { name: "/images/logos/logo-tas.svg", alt: "the avocado show" },
  { name: "/images/logos/logo-move.svg", alt: "move logo" },
  { name: "/images/logos/logo-vv.svg", alt: "vacature via logo" },
  { name: "/images/logos/logo-skybox.png", alt: "skybox logo" },
  { name: "/images/logos/logo-swb.svg", alt: "snack with benefits logo" },
];
</script>
