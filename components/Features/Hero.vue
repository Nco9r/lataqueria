<template>
  <section class="hero">
      <div class="block_top">
    <div class="hero_content">
      <div class="title_content">
        <h1>Mexican street food to BORDEAUX</h1>
        <img src="~assets/img/svg/sun.svg" alt="">
      </div>
    </div>
    <div class="description">
      <p>
        La Taqueria est un corner de restauration convivial proposant de la
        street food mexicaine de qualité, dans le respect des recettes
        traditionnelles et 100% fait maison.
      </p>
      <nuxt-link to="/">La carte</nuxt-link>
    </div>
    </div>
    <div class="block_bottom">
        <div class="img_hero">
            <img src="~assets/img/png/ambiance.jpg" alt="">
            <img class="sweet" src="~assets/img/svg/sweet_2.svg" alt="">
        </div>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style scoped>
.hero {
  margin-top: 140px;
  padding: 0 15px;
}

.hero_content {
    display: flex;
    flex-flow: row;
}

.title_content {
    position: relative;
}

.title_content h1 {
    font-size: 48px;
    line-height: 52px;
    font-weight: 500;
    position: relative;
}

.title_content img {
    position: absolute;
    top: -50px;
    right: 20px;
    width: 90px;
}

.description {
    margin-top: 10px;
}
.description p{
    font-size: 16px;
    line-height: 22px;
    margin-bottom: 20px;
}

.description a {
    color: var(--orange);
    text-transform: uppercase;
    font-family: Barbaro, 'Times New Roman', Times, serif;
    text-decoration: none;
    font-size: 18px;
}

.img_hero {
    margin-top: 20px;
    position: relative;
}

.img_hero img:nth-child(1){
    width: 100%;
    height: 400px;
    object-fit: cover;
    box-shadow: 0 12px 12px -10px rgba(37, 37, 37, 0.74);
}

.img_hero img:nth-child(2) {
    position: absolute;
    top: -50px;
    right: -10px;
    width: 150Px;
    height: 100px;
}

</style>
