components: { aboutSection, }, components: { aboutSection, },
<template>
  <nav
    class="text-white flex-row border-b py-4 sm:py-5 border-b-gray flex justify-between items-center"
  >
    <div class="text-main text-2xl lg:text-3xl gap-2 font-plexMono font-medium flex items-center">
      <div class="lg:text-3.5xl">&lt;M/&gt;</div>
      <div class="text-white">
        <h1>mohammed</h1>
      </div>
    </div>

    <div
      @click="openMenu()"
      class="text-2xl md:hidden hover:text-main transition-colors duration-200 font-bold cursor-pointer"
    >
      <span class="fa-solid fa-bars"></span>
    </div>

    <!-- Mobile navar -->
    <div
      class="bg-bgSecond h-screen fixed transition-transform duration-300 z-9999 left-0 -translate-x-full top-0 w-2xs"
      :class="{ 'translate-x-0': showMenu }"
    >
      <div class="space-y-10 py-6 px-4">
        <div
          @click="closeMenu()"
          class="text-2xl md:hidden absolute right-3 hover:text-main transition-colors duration-200 font-bold cursor-pointer"
        >
          <span class="fa-solid fa-xmark"></span>
        </div>

        <div class="text-main text-2xl gap-2 font-plexMono font-medium flex items-center">
          <div>&lt;M/&gt;</div>
          <div class="text-white">
            <h1>mohammed</h1>
          </div>
        </div>

        <ul @click="closeMenu()" class="flex flex-col items-start gap-6">
          <li
            class="text-base lg:text-xl w-full capitalize font-plexMono font-medium hover:text-main transition-colors duration-300"
          >
            <a href="#home" class="flex items-center gap-1">
              <span class="fa-solid text-main fa-home"></span>
              <span>home</span>
            </a>
          </li>
          <li
            class="text-base lg:text-xl capitalize font-plexMono font-medium hover:text-main transition-colors duration-300"
          >
            <a href="#aboutSection" class="flex items-center gap-1.5">
              <span class="fa-solid text-main fa-user"></span>
              <span>about me</span>
            </a>
          </li>
          <li
            class="text-base lg:text-xl capitalize font-plexMono font-medium hover:text-main transition-colors duration-300"
          >
            <a href="#" class="flex items-center gap-1.5">
              <span class="fa-solid text-main fa-project-diagram"></span>
              <span>projects</span>
            </a>
          </li>
        </ul>

        <ul @click="closeMenu()" class="flex items-center gap-4">
          <li
            class="font-plexMono font-medium hover:scale-125 transition-all duration-300 hover:text-main"
          >
            <a
              href="https://www.linkedin.com/in/mohammed-hussein-69a80b345"
              class="flex items-center gap-1"
              aria-label="linkedin"
            >
              <i class="fa-brands text-main text-xl fa-linkedin"></i>
            </a>
          </li>
          <li
            class="font-plexMono font-medium hover:scale-125 transition-all duration-300 hover:text-main"
          >
            <a
              href="https://github.com/Mohammed-Hussein2"
              class="flex items-center gap-1"
              aria-label="github"
            >
              <i class="fa-brands text-main text-xl fa-github"></i>
            </a>
          </li>
          <li
            class="font-plexMono font-medium hover:scale-125 transition-all duration-300 hover:text-main"
          >
            <a href="#" class="flex items-center gap-1" aria-label="whatsapp">
              <i class="fa-brands text-main text-xl fa-whatsapp"></i>
            </a>
          </li>
        </ul>
      </div>
    </div>

    <!-- tablet And Desktop navbar -->
    <div role="page links" class="hidden md:flex">
      <ul class="flex items-center gap-4 lg:gap-8">
        <li
          class="text-base lg:text-xl capitalize font-plexMono font-medium hover:text-main transition-colors duration-300"
        >
          <a href="#home" class="flex items-center gap-1">
            <span class="fa-solid text-main fa-home"></span>
            <span>home</span>
          </a>
        </li>
        <li
          class="text-base lg:text-xl capitalize font-plexMono font-medium hover:text-main transition-colors duration-300"
        >
          <a href="#aboutSection" class="flex items-center gap-1.5">
            <span class="fa-solid text-main fa-user"></span>
            <span>about me</span>
          </a>
        </li>
        <li
          class="text-base lg:text-xl capitalize font-plexMono font-medium hover:text-main transition-colors duration-300"
        >
          <a href="#projects" class="flex items-center gap-1.5">
            <span class="fa-solid text-main fa-project-diagram"></span>
            <span>projects</span>
          </a>
        </li>
      </ul>
    </div>

    <div role="socail links" class="xl:flex hidden">
      <ul class="flex items-center gap-4">
        <li
          class="font-plexMono font-medium hover:scale-125 transition-all duration-300 hover:text-main"
        >
          <a
            href="https://www.linkedin.com/in/mohammed-hussein-69a80b345"
            class="flex items-center gap-1"
            aria-label="linkedin"
          >
            <i class="fa-brands text-main text-xl fa-linkedin"></i>
          </a>
        </li>
        <li
          class="font-plexMono font-medium hover:scale-125 transition-all duration-300 hover:text-main"
        >
          <a
            href="https://github.com/Mohammed-Hussein2"
            class="flex items-center gap-1"
            aria-label="github"
          >
            <i class="fa-brands text-main text-xl fa-github"></i>
          </a>
        </li>
        <li
          class="font-plexMono font-medium hover:scale-125 transition-all duration-300 hover:text-main"
        >
          <a href="https://wa.me/01141547840" class="flex items-center gap-1" aria-label="whatsapp">
            <i class="fa-brands text-main text-xl fa-whatsapp"></i>
          </a>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      showMenu: false,
    }
  },
  methods: {
    openMenu() {
      this.showMenu = true
      document.body.classList.add('overflow-hidden')
    },
    closeMenu() {
      this.showMenu = false
      document.body.classList.remove('overflow-hidden')
    },
  },
}
</script>
