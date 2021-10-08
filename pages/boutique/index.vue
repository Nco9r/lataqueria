<template>
  <main>
      <hero/>
      <products/>
      <livraison/>
  </main>
</template>

<script>
import Hero from '../../components/Boutique/Hero.vue'
import Products from '../../components/Boutique/Products.vue'
import Livraison from '../../components/Menu/Livraison.vue'
export default {
  components: { Hero, Livraison, Products },

}
</script>

<style>

</style>