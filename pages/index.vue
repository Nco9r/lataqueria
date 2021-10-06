<template>
  <main>
    <Hero />
    <Infos/>
    <Concept/>
    <Boutique/>
    <Slide/>
    <!-- <div class="button" @click="scrollTop">
      <p>Top</p>
    </div> -->
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
  methods: {
    scrollTop() {
      window.scrollTo({
        top: 0,
        behavior: 'smooth'
      })
    }
  }
}
</script>

<style>

.button {
  position: fixed;
  bottom: 10px;
  right: 10px;
  background-color: var(--orange);
  width: 50px;
  font-weight: bold;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 50px;
  border-radius: 50%;
  z-index: 1;
}

</style>