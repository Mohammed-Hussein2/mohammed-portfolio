<template>
  <section id="aboutSection">
    <div class="layer">
      <div class="boxContainer py-12">
        <sectionIcon />
        <div
          class="grid items-center space-y-15 lg:space-x-6 xl:space-x-15 grid-cols-1 mt-32 lg:grid-cols-6"
        >
          <div class="lg:col-span-4 space-y-10">
            <h2
              class="bg-bgMain text-center md:text-start w-fit px-10 py-4 font-ubuntu font-normal text-4xl text-white border-3 border-main rounded-br-[2.5rem] rounded-tl-[2.5rem] capitalize"
            >
              about me
            </h2>

            <div
              class="bg-bgMain text-white text-base font-plexMono font-normal p-6 lg:px-10 lg:py-6 rounded-4xl space-y-2"
            >
              <span class="block text-main font-plexMono text-sm">&lt;p&gt;</span>

              <p class="text-main text-3xl font-plexMono font-medium">hello!</p>

              <p class="capitalize">
                My name is mohammed and I'm a passionate Front-End Developer specializing in
                building beautiful, responsive, and user-friendly web experiences using
                <span class="text-main">HTML </span>, <span class="text-main">CSS </span>,
                <span class="text-main">Tailwindcss </span>,
                <span class="text-main">bootstrap </span>,
                <span class="text-main">JavaScript </span>, <span class="text-main">Vue.js </span>,
                <span class="text-main">alpine.js </span>
              </p>
              <p class="capitalize">
                I'm passionate about designing perfect layouts and seamless user interactions that
                will impress them. I believe every website should be fast, easy to access, and
                enjoyable to use.
              </p>

              <span class="block text-main font-plexMono text-sm">&lt;/p&gt;</span>
            </div>
          </div>

          <div class="lg:col-span-2 mx-auto">
            <div class="rounded-2xl">
              <img
                src="../assets/images/userimage1.png"
                class="rounded-2xl xl:h-auto h-114 w-full object-cover"
                alt="about image"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import sectionIcon from './UI/sectionIcon.vue'
export default {
  components: {
    sectionIcon,
  },
}
</script>

<style scoped>
.layer {
  background-image: url(../assets/images/About.png);
  background-position: center center;
  background-size: cover;
  background-repeat: no-repeat;
}
</style>
