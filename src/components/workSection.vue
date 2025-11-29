<template>
  <section id="projects">
    <div class="layer-work">
      <div class="boxContainer relative py-16">
        <!-- Section Title -->
        <sectionIcon />
        <sectionTitle>
          <template #title> my Projects </template>
          <template #description>
            These projects were completed during my training and self learning, to improve my
            frontend skills.
          </template>
        </sectionTitle>

        <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-8 mt-12 px-4">
          <div
            v-for="(project, i) in projects"
            :key="i"
            class="bg-bgSecond rounded-xl overflow-hidden shadow-lg border border-main/10 hover:border-main transition-all duration-300"
          >
            <div class="w-full h-48 overflow-hidden">
              <img :src="project.image" :alt="project.title" class="w-full h-full object-cover" />
            </div>

            <div class="p-5 space-y-4">
              <h3 class="text-xl font-bold text-main">{{ project.title }}</h3>
              <p class="text-gray-300 text-sm leading-relaxed">{{ project.desc }}</p>
              <div class="flex items-center gap-3">
                <div v-for="(tech, i) in project.technologies" :key="i">
                  <div
                    v-text="tech"
                    class="uppercase bg-main px-2 rounded-lg font-plexMono text-sm text-bgMain font-normal"
                  ></div>
                </div>
              </div>

              <a
                :href="project.link"
                target="_blank"
                class="w-full text-center mt-3 border border-main text-main py-2 rounded-lg hover:bg-main hover:text-black capitalize flex justify-center gap-3 items-center transition duration-300"
              >
                <span>View Demo</span>
                <span class="fa-solid fa-arrow-right"></span>
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import sectionIcon from './UI/sectionIcon.vue'
import sectionTitle from './UI/sectionTitle.vue'
import CoffeeImg from '@/assets/images/Coffee.png'
import ClarityImg from '@/assets/images/Clarity.png'
import UXImg from '@/assets/images/ux.png'
import RecipeImg from '@/assets/images/recipes.png'

export default {
  components: { sectionIcon, sectionTitle },
  data() {
    return {
      projects: [
        {
          title: 'Recipe Generator',
          desc: 'A web app that generates recipe ideas dynamically, helping users discover new dishes quickly.',
          image: RecipeImg,
          technologies: ['html', 'bootstrap', 'js'],
          link: 'https://mohammed-hussein2.github.io/generator_recipes/',
        },
        {
          title: 'Clarity Digital Solution',
          desc: 'A digital solutions platform designed to enhance business operations with modern UI and responsive design.',
          image: ClarityImg,
          technologies: ['html', 'bootstrap', 'js'],
          link: 'https://mohammed-hussein2.github.io/Clarity_digital-Solution/',
        },
        {
          title: 'The UX Review',
          desc: 'A detailed UX review project showcasing user-centered design insights and interface improvements.',
          image: UXImg,
          technologies: ['html', 'css'],
          link: 'https://mohammed-hussein2.github.io/The-UX-Review/',
        },
        {
          title: 'Coffee Shop',
          desc: 'A visually appealing Coffee Shop website with smooth animations and responsive layout.',
          image: CoffeeImg,
          technologies: ['html', 'tailwindcss'],
          link: 'https://mohammed-hussein2.github.io/coffee/',
        },
      ],
    }
  },
}
</script>
<style scoped>
.layer-work {
  background-image: url(../assets/images/Works.png);
  background-size: contain;
}
</style>
