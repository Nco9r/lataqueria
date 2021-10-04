<template>
  <main>
    <Hero />
    <Infos/>
    <Concept/>
    <Boutique/>
    <Slide/>
  </main>
</template>

<script>
import Boutique from '../components/Features/Boutique.vue'
import Concept from '../components/Features/Concept.vue'
import Hero from '../components/Features/Hero.vue'
import Infos from '../components/Features/Infos.vue'
import Slide from '../components/Features/Slide.vue'
export default {
  components: {
    Hero,
    Infos,
    Concept,
    Boutique,
    Slide
  },
}
</script>

<style>

</style>