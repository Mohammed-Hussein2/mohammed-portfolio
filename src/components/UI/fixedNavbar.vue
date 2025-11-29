components: { aboutSection, },components: { aboutSection, },
<template>
  <div
    class="bg-bgSecond hidden md:flex text-white transition-all duration-200 left-1 top-1/5 rounded-[2.5rem] fixed z-99"
    :class="{ 'p-3': open }"
  >
    <div class="flex justify-center flex-col items-center gap-6">
      <div
        @click="toggle()"
        class="bg-white cursor-pointer w-10 h-10 rounded-full flex justify-center items-center"
      >
        <img src="../../assets/images/icon-grid.svg" loading="lazy" alt="Icon Grid" />
      </div>

      <ul
        class="flex transition-all duration-300 *:text-xl justify-center flex-col items-center gap-6"
        :class="{ hidden: !open }"
      >
        <li class="relative group">
          <a href="#home" class="hover:text-main transition-colors duration-300 text-xl">
            <i class="fa-solid fa-home"></i>
          </a>
          <div class="tooltip">Home</div>
        </li>

        <li class="relative group">
          <a href="#aboutSection" class="hover:text-main transition-colors duration-300 text-xl">
            <i class="fa-solid fa-user"></i>
          </a>
          <div class="tooltip">About Me</div>
        </li>

        <li class="relative group">
          <a href="#skills" class="hover:text-main transition-colors duration-300 text-xl">
            <i class="fa-solid fa-code"></i>
          </a>
          <div class="tooltip">Skills</div>
        </li>

        <li class="relative group">
          <a href="#projects" class="hover:text-main transition-colors duration-300 text-xl">
            <i class="fa-solid fa-tv"></i>
          </a>
          <div class="tooltip">Projects</div>
        </li>

        <li class="relative group">
          <a
            href="mailto:mohammedhussein2512m@gmail.com"
            class="hover:text-main transition-colors duration-300 text-xl"
          >
            <i class="fa-solid fa-envelope"></i>
          </a>
          <div class="tooltip">Contact</div>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      open: true,
    }
  },
  methods: {
    toggle() {
      this.open = !this.open
    },
  },
}
</script>
