<template>
  <section class="hero">
    <div class="block_top">
      <div class="hero_content">
        <div class="title_content">
          <h1>DECOUVREz NOTRE CARTE</h1>
          <img src="~assets/img/svg/sun.svg" alt="" />
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
        <img src="~assets/img/png/ambiance_2.jpg" alt="" />
        <img class="sweet" src="~assets/img/svg/sweet_2.svg" alt="" />
        <!-- <img class="sweet" src="~assets/img/svg/sun_2.svg" alt="" />
        <img class="sweet" src="~assets/img/svg/sun_2.svg" alt="" /> -->
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
  padding-right: 30px;
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
.description p {
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

.img_hero img:nth-child(1) {
  width: 100%;
  height: 400px;
  object-fit: cover;
  box-shadow: 0 12px 12px -10px rgba(37, 37, 37, 0.74);
}

.img_hero img:nth-child(2) {
  position: absolute;
  top: -50px;
  right: -10px;
  width: 150px;
  height: 100px;
}

@media screen and (min-width: 1024px) {
.hero {
  max-width: 1000px;
  margin: 180px auto 30px auto;
}

  .block_top {
    display: flex;
    flex-flow: row wrap;
    justify-content: space-between;
  }

  .hero_content {
    width: 49%;
  }

  

  .title_content h1 {
  font-size: 70px;
  line-height: 75px;
  padding-right: 30px;
  font-weight: 500;
  position: relative;
}

.title_content img {
  position: absolute;
  top: -70px;
  right: 0px;
  width: 130px;
}

  .description {
    width: 49%;
  }

  .description p {
  font-size: 20px;
  line-height: 28px;
  margin-bottom: 20px;
}

.img_hero img:nth-child(2) {
  position: absolute;
  top: -50px;
  right: -10px;
  width: 190px;
  height: 140px;
}

.img_hero img:nth-child(4) {
  position: absolute;
   bottom: -110px;
  right: -10px;
    transform: rotate(270deg);

  width: 50px;
  height: 200px;
}


  
  .img_hero img:nth-child(3) {
    width: 50px;
    position: absolute;
    bottom: -30px;
    transform: rotate(334deg);
    left: -10px;
  }
}

@media screen and (min-width: 1200px) {
.hero {
  max-width: 1200px;
  margin: 180px auto 50px auto;
}

  .title_content h1 {
  font-size: 80px;
  line-height: 85px;
  padding-right: 30px;
  font-weight: 500;
  position: relative;
}


.img_hero img:nth-child(1) {
  height: 550px;
  margin-top: 20px;
}

.title_content img {
  position: absolute;
  top: -80px;
  right: 30px;
  width: 170px;
}

.img_hero img:nth-child(4) {
  position: absolute;
   bottom: -130px;
  right: 0px;
    transform: rotate(290deg);

  width: 80px;
  height: 200px;
}


  
  .img_hero img:nth-child(3) {
    width: 50px;
    position: absolute;
    bottom: -30px;
    transform: rotate(334deg);
    left: -10px;
  }

}

@media screen and (min-width: 1440px) {
.hero {
  max-width: 1300px;
  margin: 200px auto 50px auto;
}

  .title_content h1 {
  font-size: 85px;
  line-height: 90px;
  padding-right: 30px;
  font-weight: 500;
  position: relative;
}

}
@media screen and (min-width: 1600px) {
.hero {
  max-width: 1600px;
  margin: 180px auto 50px auto;
}


.title_content img {
  position: absolute;
  top: -80px;
  right: -50px;
  width: 170px;
}}
</style>
