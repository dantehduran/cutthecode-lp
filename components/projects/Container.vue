<template>
  <section class="md:pt-24 px-5 mx-auto">
    <div
      class="bg-muted text-muted-foreground rounded-t-3xl rounded-bl-2xl relative pt-24 pb-12"
    >
      <div
        class="flex gap-3 w-full overflow-hidden min-w-fit whitespace-nowrap px-16"
      >
        <div
          class="w-80 flex-shrink-0 flex flex-col gap-6 cursor-pointer"
        ></div>
      </div>
    </div>
  </section>
</template>
<script setup lang="ts">
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
