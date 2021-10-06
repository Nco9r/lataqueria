<template>
  <section class="livraison">
      <h2>Faites vous livrez</h2>
      <a href="https://deliveroo.fr/fr/menu/bordeaux/bordeaux-gare-nansouty/la-taqueria-la-boca-foodcourt" target="_blank"><button>Commandez</button></a>
  </section>
</template>

<script>
export default {

}
</script>

<style scoped>

.livraison {
    height: 350px;
    background-image: url('~assets/img/png/store_1.jpg');
    background-size: 150%;
    display: flex;
    flex-flow: column;
    justify-content: center;
    align-items: center;
    background-position: 50% 50% ;
    background-repeat: no-repeat;
}

.livraison h2 {
    font-size: 41px;
text-shadow: 0 12px 12px -10px rgba(8, 8, 8, 0.842);

}

.livraison button {
      border: none;
  padding: 16px 58px;
  background-color: var(--orange);
  color: var(--white);
  font-size: 16px;
  margin-top: 20px;
  position: relative;
}

</style>