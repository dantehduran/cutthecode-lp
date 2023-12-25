<template>
  <div
    class="leading-relaxed md:leading-none antialiased bg-background font-sans min-h-full dark mt-2"
  >
    <HeaderNotification />
    <HeaderNav />
    <main class="z-0 relative bg-background">
      <section>
        <div class="px-5 mx-auto w-full">
          <div
            class="bg-muted relative overflow-hidden rounded-t-3xl rounded-bl-3xl"
          >
            <div class="px-8 md:w-full md:px-16">
              <div class="mx-auto w-full max-w-[96rem]">
                <div class="px-6 md:px-8 pt-28 md:pt-36 flex flex-col gap-4">
                  <div class="flex gap-4 justify-start items-center">
                    <Dot class="text-primary scale-150" />
                    <span class="font-extrabold text-lg leading-5 capitalize"
                      >leading No-Code & webflow agency</span
                    >
                  </div>
                  <h2 class="text-8xl tracking-wide">
                    We enable rapid growth through digital creation
                  </h2>
                  <div class="flex justify-between items-end pb-4 w-full">
                    <div class="opacity-80 w-2/5 text-lg font-semibold">
                      Cut the Code is a leading no-code agency & Webflow Partner
                      based in Amsterdam, The Netherlands. We push our clients
                      forward into tomorrow - and fast - by creating the next
                      generation of web experiences.
                    </div>
                    <div class="w-1/4 flex gap-4 justify-center items-end">
                      <div class="min-w-fit">
                        <img
                          src="~/assets/logos/partner-wf.svg"
                          alt="partner wf"
                        />
                      </div>
                      <div class="flex justify-center items-center">
                        <CustomButton class="bg-white text-background"
                          >Learn more
                          <template #icon
                            ><svg
                              height="100%"
                              viewBox="0 0 15 18"
                              fill="none"
                              xmlns="http://www.w3.org/2000/svg"
                            >
                              <path
                                d="M8.46009 0.277253L8.20565 14.8126L9.03122 14.8258C9.20577 13.8891 9.7077 13.0326 10.4588 12.3896L13.3614 9.77656L14.525 10.8997L7.29573 17.4076L0.332226 10.6856L1.53713 9.60089L4.25203 12.2216C5.02837 12.895 5.52057 13.8051 5.63975 14.7874L6.50104 14.8014L6.77329 0.25L8.46009 0.277253Z"
                                fill="currentColor"
                              ></path></svg
                          ></template>
                        </CustomButton>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
    </main>
  </div>
</template>
<script setup lang="ts">
useHead({
  title: "No-Code Agency & Webflow Partner for Ambitious Brands",
  meta: [{ name: "description", content: "No-Code landing page" }],
  bodyAttrs: {
    class: "dark",
  },
});
</script>
