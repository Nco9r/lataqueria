<template>
  <main>
      <hero/>
      <carte/>
      <livraison/>
  </main>
</template>

<script>
import Hero from '../../components/Menu/Hero.vue'
import Carte from '../../components/Menu/Carte.vue'
import Livraison from '../../components/Menu/Livraison.vue'

export default {
  components: { Hero, Carte, Livraison },

}
</script>

<style>

</style>