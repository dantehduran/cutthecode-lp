<template>
  <div class="absolute h-4 w-4">
    <svg viewBox="0 0 16 16" xmlns="http://www.w3.org/2000/svg">
      <mask id="my-mask">
        <rect fill="white" width="16" height="16"></rect>
        <circle fill="black" cx="16" cy="16" r="16" />
      </mask>
      <rect
        mask="url(#my-mask)"
        x="0"
        y="0"
        width="16"
        height="16"
        fill="currentColor"
      ></rect>
    </svg>
  </div>
</template>
