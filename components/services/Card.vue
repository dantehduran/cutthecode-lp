<template>
  <div
    class="group relative rounded-2xl w-full pr-6 py-8 pl-8 border-r border-r-primary/30"
  >
    <div
      class="absolute w-full h-full inset-0 rounded-2xl bg-gradient-to-tl from-primary/20 opacity-0 group-hover:opacity-20"
    ></div>
    <div class="flex flex-col gap-4 relative transform transition-all">
      <div class="flex items-center gap-4">
        <div class="w-16 scale-0 group-hover:scale-100 duration-200 ease-out">
          <img :src="'/images/' + icon" alt="" />
        </div>
        <h4
          class="text-4xl capitalize font-light -translate-x-20 group-hover:translate-x-0 duration-500 ease-out"
        >
          {{ title }}
        </h4>
      </div>
      <div class="text-opacity-60 font-sans font-normal w-4/5">
        {{ description }}
      </div>
      <div
        class="absolute w-12 h-12 rounded-full flex justify-center items-center right-0 bottom-0 bg-gradient-to-tl from-primary/20"
      >
        <div
          class="flex justify-center items-center w-5 group-hover:-rotate-180 duration-200 ease-in"
        >
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
      </div>
    </div>
  </div>
</template>
<script setup lang="ts">
defineProps({
  title: String,
  description: String,
  icon: String,
});
</script>
