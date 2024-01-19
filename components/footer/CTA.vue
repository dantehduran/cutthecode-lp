<template>
  <div class="w-full h-56 flex items-center overflow-hidden group">
    <div class="whitespace-nowrap telepromt flex max-w-fit gap-8">
      <div class="flex gap-8 items-center" v-for="n in 4" :key="n">
        <div class="h-12 w-12 text-muted">
          <svg
            height="100%"
            viewBox="0 0 24 23"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M15.7196 11.9163C13.8735 11.9163 12.3279 13.3863 12.3279 15.2342V22.5H11.641V15.2342C11.641 13.3863 10.0954 11.9163 8.20639 11.9163H0.822021V11.2443H8.20639C10.0954 11.2023 11.641 9.73237 11.5981 7.88442V0.660645H12.3279V7.88442C12.3279 9.73237 13.8735 11.2023 15.7196 11.2023H23.1469V11.9163H15.7196Z"
              fill="currentColor"
            ></path>
          </svg>
        </div>
        <h3 class="text-5xl tracking-wider text-primary-foreground pb-2">
          Ready to move faster?
        </h3>
        <CustomButton class="bg-muted text-muted-foreground"
          >Get in touch<template #icon
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
</template>
<style scoped>
.group:hover .telepromt {
  animation-play-state: paused;
}
</style>
