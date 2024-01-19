<template>
  <section class="mt-24">
    <div class="bg-primary w-full rounded-t-3xl">
      <FooterCTA />
      <div class="px-5">
        <div
          class="relative pt-40 pb-24 px-16 mx-auto rounded-t-2xl bg-muted w-full"
        >
          <div class="absolute w-14 text-primary top-16">
            <svg
              width="100%"
              viewBox="0 0 52 53"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M32.4277 25.4909L46.0625 25.4909C47.4882 25.4908 48.8642 24.9636 49.9284 24.0097C50.9926 23.0557 51.6707 21.7417 51.8337 20.3177V5.75581C51.8336 4.39018 51.2939 3.0805 50.3334 2.11486C49.3729 1.14921 48.0702 0.606635 46.7118 0.606503L5.73861 0.606503C4.3802 0.606503 3.0774 1.14906 2.11686 2.11473C1.15631 3.08041 0.616699 4.39014 0.616699 5.75581L0.616699 46.9479C0.616634 47.6241 0.749054 48.2937 1.00643 48.9184C1.26381 49.5432 1.64108 50.1109 2.1167 50.5891C2.59233 51.0673 3.15701 51.4465 3.77846 51.7053C4.39991 51.964 5.06598 52.0971 5.73861 52.0971H46.7123C47.385 52.0971 48.051 51.9639 48.6724 51.7051C49.2938 51.4464 49.8585 51.0671 50.3341 50.589C50.8097 50.1108 51.1869 49.5432 51.4443 48.9184C51.7017 48.2937 51.8342 47.6241 51.8342 46.9479V35.3756V32.7404C51.6703 31.3172 50.992 30.0041 49.9283 29.0506C48.8646 28.0972 47.4896 27.5698 46.0645 27.5686L32.4287 27.5686C30.8883 27.5696 29.4113 28.1851 28.322 29.2802C27.2327 30.3752 26.6203 31.86 26.6192 33.4086V34.5556L26.6122 35.8177V38.0751C26.6122 38.6049 26.1827 39.0344 25.6529 39.0344V39.0344C25.1233 39.0344 24.6939 38.6054 24.6935 38.0759L24.6889 33.0445V32.996L24.6889 19.7096V19.5914L24.6935 14.6315C24.6939 14.1015 25.1237 13.6722 25.6537 13.6722V13.6722C26.1833 13.6722 26.613 14.1011 26.6139 14.6308L26.6192 17.8118L26.6122 18.6255L26.6192 19.6524C26.6207 21.2006 27.2331 22.685 28.3222 23.7797C29.4112 24.8743 30.8878 25.4898 32.4277 25.4909Z"
                fill="currentColor"
              ></path>
            </svg>
          </div>
          <div class="grid grid-cols-[.5fr_1fr] justify-between gap-[8vw]">
            <div class="flex flex-col w-full max-w-md gap-6">
              <div class="flex gap-4 justify-start items-center">
                <Dot class="bg-primary scale-150" />
                <h6 class="text-2xl font-semibold">
                  Want to receive no-code news and updates?
                </h6>
              </div>
              <form action="submit" class="flex flex-col gap-4">
                <input
                  type="text"
                  name="name"
                  placeholder="Name"
                  maxlength="256"
                  required
                  class="w-full min-h-[3.25rem] bg-background border-background rounded-2xl py-2 px-5 hover:border-primary focus:border-primary focus:outline-none focus:ring-0 transition-all duration-200 ease-in-out"
                />
                <input
                  type="email"
                  name="email"
                  placeholder="Email"
                  maxlength="256"
                  required
                  class="w-full min-h-[3.25rem] bg-background border-background rounded-2xl py-2 px-5 hover:border-primary focus:border-primary focus:outline-none focus:ring-0 transition-all duration-200 ease-in-out"
                />
                <div class="flex gap-2 items-center">
                  <input
                    type="checkbox"
                    class="text-primary bg-background rounded-full focus:outline-none focus:ring-0"
                  />
                  <h6 class="text-sm">
                    I agree with the
                    <span class="text-primary font-semibold"
                      >privacy statement</span
                    >
                  </h6>
                </div>
                <div class="flex max-w-fit mt-4">
                  <CustomButton class="bg-primary text-primary-foreground"
                    >Get the latest updates<template #icon
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
              </form>
            </div>
            <div class="flex flex-col justify-between items-center pl-10">
              <div class="flex justify-evenly items-start gap-24">
                <div class="flex flex-col gap-2 items-start justify-start">
                  <h6 class="opacity-60 mb-2">Services</h6>
                  <div
                    v-for="service in services"
                    :key="service"
                    class="flex items-center justify-start gap-2 transition-all group"
                  >
                    <Dot
                      class="scale-0 group-hover:scale-100 duration-200 ease-out"
                    />
                    <span
                      class="capitalize text-lg cursor-pointer font-semibold -translate-x-3.5 group-hover:translate-x-0 duration-200 ease-in-out"
                      >{{ service }}</span
                    >
                  </div>
                </div>
                <div class="flex flex-col gap-2 items-start justify-start">
                  <h6 class="opacity-60 mb-2">Company</h6>
                  <div
                    v-for="item in company"
                    :key="item"
                    class="flex items-center justify-start gap-2 transition-all group"
                  >
                    <Dot
                      class="scale-0 group-hover:scale-100 duration-200 ease-out"
                    />
                    <span
                      class="capitalize text-lg cursor-pointer font-semibold -translate-x-3.5 group-hover:translate-x-0 duration-200 ease-in-out"
                      >{{ item }}</span
                    >
                  </div>
                </div>
                <div class="flex flex-col gap-4">
                  <h6 class="opacity-60 mb-2">Company</h6>
                  <div class="flex flex-col gap-2">
                    <h6 enter-class="text-lg font-bold capitalize">
                      Armsterdam
                    </h6>
                    <span class="opacity-80 hover:text-primary"
                      >Wibautstraat 131 D1091 GL Amsterdam</span
                    >
                  </div>
                  <div class="flex flex-col gap-2">
                    <h6 enter-class="text-lg font-bold capitalize">Zwolle</h6>
                    <span class="opacity-80 hover:text-primary"
                      >Burgemeester Roelenweg 118021 EV Zwolle</span
                    >
                  </div>
                </div>
              </div>
              <FooterSocials />
            </div>
          </div>
          <div
            class="absolute max-w-[25%] text-primary top-0 left-[40vw] -translate-x-[50%]"
          >
            <svg
              width="100%"
              viewBox="0 0 327 152"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M173.442 -63.8074L173.24 -163.122C173.229 -168.72 168.7 -173.258 163.102 -173.28C157.457 -173.302 152.872 -168.725 152.884 -163.08L153.093 -63.899C153.124 -58.2765 152.035 -52.7113 149.889 -47.5277C147.742 -42.3442 144.583 -37.644 140.592 -33.7022C136.626 -29.7194 131.897 -26.5709 126.685 -24.4379C121.473 -22.3049 115.882 -21.2299 110.234 -21.2784L10.8028 -21.7808C5.1631 -21.8093 0.580995 -17.2359 0.59876 -11.5962C0.616322 -6.02135 5.12574 -1.50349 10.7005 -1.47551L110.317 -0.975429C121.687 -0.882664 132.59 3.69421 140.644 11.7555C148.699 19.8167 153.249 30.7066 153.304 42.0475L153.507 141.321C153.519 146.915 158.043 151.451 163.637 151.476C169.282 151.501 173.869 146.926 173.858 141.281L173.669 42.1164C173.696 30.7926 178.21 19.9711 186.225 12.0075C194.24 4.04379 205.107 -0.416526 216.46 -0.400555L315.916 0.0969614C321.552 0.125153 326.131 -4.44324 326.116 -10.0787C326.102 -15.6535 321.593 -20.173 316.019 -20.2013L216.395 -20.7067C205.019 -20.8092 194.112 -25.4018 186.063 -33.4784C178.015 -41.555 173.476 -52.4597 173.442 -63.8074Z"
                fill="currentColor"
              ></path>
            </svg>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script setup lang="ts">
const services = ["design", "build", "automate", "no-code"];
const company = ["projects", "about us", "careers", "contact"];
</script>
