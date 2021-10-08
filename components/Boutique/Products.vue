<template>
  <section class="products">
    <div class="products_hr">
      <hr />
      <div class="items_products" @click="display = !display">
        <h2>Tous nos produits</h2>
        <h2 v-if="partage">A partager</h2>
        <h2 v-if="plus">Boissons</h2>
        <img src="~assets/img/svg/select_orange.svg" alt="" />
      </div>
      <p class="offer" v-if="display">Découvrer égalements</p>
      <div class="items_menu_display" v-if="display">
        <h2
          @click="
            ;(partage = false),
              (plats = true),
              (plus = false),
              (display = !display)
          "
          v-if="!plats"
        >
          Nos plats
        </h2>
        <h2
          @click="
            ;(partage = true),
              (plats = false),
              (plus = false),
              (display = !display)
          "
          v-if="!partage"
        >
          a partager
        </h2>
        <h2  @click="
            ;(partage = false),
              (plats = false),
              (plus = true),
              (display = !display)
          "
          v-if="!plus">Boissons</h2>
      </div>
      <hr />
    </div>
  </section>
</template>

<script>
export default {

}
</script>

<style scoped>

.products {
  background-color: var(--white);
  margin-top: -200px;
  padding-bottom: 50px;
  height: 1000Px;
  background-image: url('assets/img/svg/bck.svg');
  background-repeat: repeat;
  background-size: 250%;
}

.products_hr {
    padding: 250px 20px 20px 20px;
}

.items_products {
     position: sticky;
  background-color: var(--white);
  top: 150px;
  display: flex;
  justify-content: space-between;
  padding: 20px;

}

.items_products h2 {
  font-size: 28px;
  -webkit-text-stroke: 1px var(--orange);
  color: transparent;
}

</style>