<template>
  <section class="md:pt-24 px-5 mx-auto">
    <div
      class="bg-muted text-muted-foreground rounded-t-3xl rounded-bl-2xl relative pt-24 pb-12"
    >
      <div
        class="flex gap-3 w-full overflow-x-hidden whitespace-nowrap px-16 scroll-smooth snap-x snap-mandatory scroll-pl-16"
        ref="scrollRef"
      >
        <ProjectsCard
          v-for="(item, index) in data"
          :key="index"
          v-bind="item"
          class="snap-start snap-always"
        />
      </div>
    </div>
    <div class="h-24 flex justify-end relative -top-0.5 items-start">
      <div class="w-full h-full relative -right-0.5 bg-background">
        <Curve class="text-muted absolute top-0 right-0 rotate-90" />
      </div>
      <div
        class="h-full w-80 bg-muted rounded-b-2xl flex justify-center items-center"
      >
        <div class="flex gap-6 items-center justify-end text-red-800">
          <button
            @click="scrollLeft"
            class="cursor-pointer w-12 h-12 rounded-2xl bg-background text-foreground flex justify-center items-center"
          >
            <div class="h-4 flex justify-center items-center rotate-180">
              <svg
                height="100%"
                viewBox="0 0 22 18"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M0.306828 8.34796L18.1265 8.32769C18.4155 8.32737 18.6495 8.09298 18.6494 7.80402V7.80402C18.6493 7.54607 18.4606 7.32932 18.2098 7.26876C17.1956 7.02383 16.2699 6.49123 15.5465 5.73061L12.1904 2.37452L13.5835 0.981431L21.9421 9.34008L13.6046 17.6776L12.2115 16.2844L15.4621 13.0338C16.1897 12.2239 17.1494 11.6646 18.2042 11.4279C18.4686 11.3686 18.6704 11.1426 18.6704 10.8717V10.8717C18.6704 10.5737 18.4289 10.3321 18.1308 10.3321L0.307074 10.3323L0.306828 8.34796Z"
                  fill="currentColor"
                ></path>
              </svg>
            </div>
          </button>

          <button
            @click="scrollRight"
            class="cursor-pointer w-12 h-12 rounded-2xl bg-background text-foreground flex justify-center items-center"
          >
            <div class="h-4 flex justify-center items-center">
              <svg
                height="100%"
                viewBox="0 0 22 18"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M0.306828 8.34796L18.1265 8.32769C18.4155 8.32737 18.6495 8.09298 18.6494 7.80402V7.80402C18.6493 7.54607 18.4606 7.32932 18.2098 7.26876C17.1956 7.02383 16.2699 6.49123 15.5465 5.73061L12.1904 2.37452L13.5835 0.981431L21.9421 9.34008L13.6046 17.6776L12.2115 16.2844L15.4621 13.0338C16.1897 12.2239 17.1494 11.6646 18.2042 11.4279C18.4686 11.3686 18.6704 11.1426 18.6704 10.8717V10.8717C18.6704 10.5737 18.4289 10.3321 18.1308 10.3321L0.307074 10.3323L0.306828 8.34796Z"
                  fill="currentColor"
                ></path>
              </svg>
            </div>
          </button>
        </div>
      </div>
    </div>
  </section>
</template>
<script setup lang="ts">
import { ref, onMounted } from "vue";

const scrollRef = ref<HTMLElement | null>(null);
let scrollContainer: HTMLElement;

const scrollLeft = () => {
  scrollContainer.scrollLeft -= 320;
};

const scrollRight = () => {
  scrollContainer.scrollLeft += 320;
};

onMounted(() => {
  if (scrollRef.value) {
    scrollContainer = scrollRef.value;
  }
});

const data = [
  {
    img: "/projects/reducations.webp",
    client: "reducations",
    desc: "A new era of education at the Dutch Creative Technology Academy",
    case: true,
  },
  {
    img: "/projects/skybox.webp",
    client: "skybox x samsung",
    desc: "Let's inspire the future with a free online academy",
    case: false,
  },
  {
    img: "/projects/vita.webp",
    client: "vacatura vita",
    desc: "Building the world’s most advanced no-code job platform",
    case: true,
  },
  {
    img: "/projects/snack.webp",
    client: "snack with benefits",
    desc: "A plant-based experience that looks as good as it tastes ",
    case: true,
  },
  {
    img: "/projects/agency.webp",
    client: "for you agency",
    desc: "reaching the next gen like no other",
    case: false,
  },
  {
    img: "/projects/caya.webp",
    client: "caya",
    desc: "taking document management international in just 2 weeks",
    case: true,
  },
  {
    img: "/projects/avocado.webp",
    client: "the avocado show",
    desc: "a new scalable, digital footprint for the avocado show",
    case: false,
  },
  {
    img: "/projects/skybox2.webp",
    client: "skybox",
    desc: "in just one month from scratch to a creative platform",
    case: true,
  },
  {
    img: "/projects/move.webp",
    client: "move agency",
    desc: "a digital experience for the largest mobile agency of the netherlands",
    case: false,
  },
  {
    img: "/projects/springplank.webp",
    client: "springplank",
    desc: "a landingpage for the youngest generation of hard workers",
    case: false,
  },
  {
    img: "/projects/oneup.webp",
    client: "oneUp",
    desc: "a outspoken design to reflect the disruptive character",
    case: false,
  },
];
</script>
