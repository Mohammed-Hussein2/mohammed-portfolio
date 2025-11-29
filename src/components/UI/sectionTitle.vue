<template>
  <div class="mx-auto text-center space-y-6 mt-15">
    <h2 class="font-ubuntu capitalize w-fit mx-auto relative font-normal text-6xl text-main">
      <slot name="title"></slot>
      <div class="absolute w-full h-0.5 mt-2.5 bg-main">
        <div class="w-3 h-3 rounded-full bg-main absolute top-1/2 -translate-y-1/2 left-0"></div>
        <div class="w-3 h-3 rounded-full bg-main absolute top-1/2 -translate-y-1/2 right-0"></div>
      </div>
    </h2>

    <p class="text-base font-plexMono font-normal text-white">
      <slot name="description"></slot>
    </p>
  </div>
</template>
