<template>
  <button
    :class="buttonClass"
    class="flex items-center text-base md:text-xl transition-colors duration-300 px-2 py-4 md:py-4 md:px-8 min-w-53 rounded-4xl justify-center gap-4 cursor-pointer"
  >
    <slot></slot>
  </button>
</template>

<script>
export default {
  name: 'baseButton',
  props: {
    buttonClass: {
      type: String,
      default: 'bg-main',
    },
  },
}
</script>
