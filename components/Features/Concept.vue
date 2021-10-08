<template>
  <section class="concept">
    <div class="block_left">
      <img src="~assets/img/png/nachos.jpg" alt="" />
      <img src="~assets/img/svg/sun_3.svg" alt="" />
      <div class="box"></div>
    </div>
    <div class="block_right">
      <div class="title_concept">
        <h2>Choisissez votre Formule.</h2>
      </div>
      <div class="content_concept">
        <p>Comment ça marche ?</p>
        <p>
          Choisissez le format de votre plat parmi : Maxi Burrito, Quesadillas,
          Tacos, Bowl Mexicain. <br />
          Puis choisissez votre garnitures dans les suggestions du moment.
          Effiloché de boeuf braisé à la bière. Effiloché de porc laqué à la
          mangue. Poulet mariné salsa verde. Crevettes grillés épices douces
          sauce Pipian. Végétarien.s
        </p>
      </div>
      <div class="btn_concept">
        <nuxt-link to="/menu">
          <button>La carte</button>
        </nuxt-link>
      </div>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style scoped>
.concept {
  padding: 10px 20px 20px 20px;
  background-image: url('~assets/img/svg/sun_bck.svg');
  background-size: 200%;
  background-position: 45% 110%;
  background-repeat: no-repeat;
}

.block_left {
  position: relative;
}

.block_left img {
  width: 85%;
  height: 350px;
  object-fit: cover;
}

.block_left img:nth-child(2) {
  position: absolute;
  width: 90px;
  top: 15%;
  right: 30%;
  height: 60px;
}

.box {
  border: 8px double var(--yellow);
  width: 250px;
  position: absolute;
  height: 320px;
  top: 15px;
  right: 0;
}

.block_right .title_concept h2 {
  margin-top: 30px;
  font-size: 35px;
  line-height: 43px;
  font-weight: 500;
}

.content_concept p:nth-child(1) {
  font-family: ColabMed, sans-serif;
  font-size: 18px;
  margin-top: 20px;
  margin-bottom: 10px;
}

.content_concept p:nth-child(2) {
  font-size: 16px;
  line-height: 22px;
  margin-bottom: 20px;
}

br {
  margin-bottom: 10px;
}

.btn_concept button {
  border: none;
  padding: 16px 58px;
  background-color: var(--orange);
  color: var(--white);
  font-size: 16px;
  position: relative;
}

@media screen and (min-width: 1024px) {
  .concept {
  max-width: 1000px;
  background-size: 50%;

  margin: 30px auto 100px auto;
  display: flex;
  flex-flow: row-reverse;
  align-items: flex-start;
  justify-content: space-between;
}
.block_right {
  width: 45%;
}

.block_left {
  width: 45%;
}
.block_right .title_concept h2 {
  margin-top: 30px;
  font-size: 48px;
  line-height: 52px;

}

.content_concept p:nth-child(1) {
  font-size: 24px;
  line-height: 32px;
}

.content_concept p:nth-child(2) {
  font-size: 20px;
  line-height: 28px;
}
}

@media screen and (min-width: 1200px) {
  .concept {
  max-width: 1150px;
  background-size: 45%;

  margin: 30px auto 100px auto;
  display: flex;
  flex-flow: row-reverse;
  align-items: flex-start;
  justify-content: space-between;
}
.block_right {
  width: 45%;
}

.block_left {
  width: 45%;
}
.block_right .title_concept h2 {
  margin-top: 30px;
  font-size: 48px;
  line-height: 52px;
}


}
</style>
