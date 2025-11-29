<template>
  <header class="boxContainer">
    <theNavbar></theNavbar>
    <fixedNavbar />
  </header>
  <main>
    <mainSection />
    <aboutSection />
    <skillsSection />
    <workSection />
    <theFooter />
  </main>
</template>

<script>
import theNavbar from '@/components/theNavbar.vue'
import mainSection from '@/components/mainSection.vue'
import aboutSection from '@/components/aboutSection.vue'
import skillsSection from '@/components/skillsSection.vue'
import workSection from '@/components/workSection.vue'
import fixedNavbar from '@/components/UI/fixedNavbar.vue'
import theFooter from '@/components/theFooter.vue'
export default {
  components: {
    theNavbar,
    mainSection,
    aboutSection,
    skillsSection,
    workSection,
    theFooter,
    fixedNavbar,
  },
}
</script>
