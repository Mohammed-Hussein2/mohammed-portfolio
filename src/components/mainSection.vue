<template>
  <section id="home" class="boxContainer py-6 space-y-16">
    <div class="hidden md:flex md:justify-center md:items-center">
      <h2 class="text-8xl text-second font-ubuntu font-normal">developer</h2>
    </div>

    <div class="grid grid-cols-1 lg:gap-18 space-y-10 lg:grid-cols-5">
      <div class="col-span-2">
        <div
          class="border-3 border-white p-4 max-w-103 mx-auto"
          style="border-radius: 160px 0 160px 0; box-shadow: -4px -4px 2px 0 #12f7d6"
        >
          <div class="flex flex-col mb-7 items-center">
            <img
              src="../assets/images/userImage.jpg"
              class="w-24 h-24 border-3 rounded-full border-main object-cover"
              alt="user image"
              loading="lazy"
            />
            <h3 class="mt-3 text-3xl font-plexMono font-medium text-white">Mohammed</h3>
            <p class="font-plexMono font-normal text-base text-white">Front-end developer</p>
          </div>

          <div>
            <ul class="space-y-2">
              <li class="text-white text-sm font-plexMono font-normal">
                <a class="flex items-center gap-2" href="mailto:mohammedhussein2512m@gmail.com">
                  <i class="text-main text-base fa-regular fa-envelope"></i>
                  <span>mohammedhussein2512m@gmail.com</span>
                </a>
              </li>
              <li class="text-white text-sm font-plexMono font-normal">
                <a
                  class="flex items-center gap-2"
                  href="https://www.linkedin.com/in/mohammed-hussein-69a80b345"
                >
                  <i class="text-main text-base fa-brands fa-linkedin"></i>
                  <span>Linked In</span>
                </a>
              </li>
              <li class="text-white text-sm font-plexMono font-normal">
                <a class="flex items-center gap-2" href="https://github.com/Mohammed-Hussein2">
                  <i class="text-main text-base fa-brands fa-github"></i>
                  <span>GitHub</span>
                </a>
              </li>
              <li class="text-white text-sm font-plexMono font-normal">
                <div class="flex items-center gap-2">
                  <i class="text-main text-base fa-solid fa-location-dot"></i>
                  <span>Egypt/Giza</span>
                </div>
              </li>
            </ul>
          </div>

          <div>
            <ul class="flex items-center gap-4 flex-wrap mt-7">
              <li
                class="capitalize bg-main px-2 rounded-lg font-plexMono text-sm text-bgMain font-normal"
              >
                HTML5
              </li>
              <li
                class="capitalize bg-main px-2 rounded-lg font-plexMono text-sm text-bgMain font-normal"
              >
                CSS3
              </li>
              <li
                class="capitalize bg-main px-2 rounded-lg font-plexMono text-sm text-bgMain font-normal"
              >
                JS
              </li>
              <li
                class="capitalize bg-main px-2 rounded-lg font-plexMono text-sm text-bgMain font-normal"
              >
                Vue.JS
              </li>
              <li
                class="capitalize bg-main px-2 rounded-lg font-plexMono text-sm text-bgMain font-normal"
              >
                TailwindCSS
              </li>
              <li
                class="capitalize bg-main px-2 rounded-lg font-plexMono text-sm text-bgMain font-normal"
              >
                bootstrap
              </li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-span-3">
        <div class="space-y-8">
          <h2
            class="text-white capitalize font-ubuntu font-medium text-3xl md:text-6xl leading-9 md:leading-18"
          >
            <span class="block text-main font-plexMono lowercase text-sm -ml-4">&lt;h2&gt;</span>
            <p class="block">hey</p>
            <p>i'm <span class="text-main">Mohammed</span></p>
            <p>Front-end Developer</p>
            <span class="block text-main lowercase font-plexMono text-sm -ml-4">&lt;h2&gt;</span>
          </h2>

          <p class="font-plexMono font-normal text-base text-white">
            <span class="block text-main font-plexMono text-sm -ml-4 mb-2.5">&lt;p&gt;</span>
            I enjoy solving UI problems, improving user experience, and writing code that’s readable
            and maintainable.
            <span class="block text-main font-plexMono text-sm -ml-4 mt-2.5">&lt;/p&gt;</span>
          </p>

          <div
            class="flex lg:mt-9 justify-start flex-col md:flex-row space-y-4 md:space-y-0 items-center md:gap-3"
          >
            <a href="#projects" class="font-plexMono capitalize font-normal">
              <baseButton> view Projects </baseButton>
            </a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import baseButton from '@/components/UI/baseButton.vue'
export default {
  components: {
    baseButton,
  },
}
</script>

<style></style>
