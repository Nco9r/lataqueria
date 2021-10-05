<template>
  <section class="slide">
    <div class="img_welcome">
      <img src="~assets/img/svg/pic.svg" alt="" />
    </div>
    <div class="title_slide">
        <img src="~assets/img/svg/sun.svg" alt="">
      <h2>Mexican street food to BORDEAUX</h2>
    </div>
    <div class="slide_mobile">
        <img src="~assets/img/svg/tequila.svg" alt="">
    </div>
    <div class="slide_tiny">
        <img src="~assets/img/png/quesadillas.jpg" alt="">
        <h3>quesadillas</h3>
    </div>
    <div class="btn_slide">
      <button>Voir la Carte</button>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style scoped>
.slide {
  background-color: var(--white);
  background-image: url('assets/img/svg/bck.svg');
  background-repeat: repeat;
  background-size: 250%;
  overflow: hidden;
  position: relative;
}



.img_welcome img {
  width: 200px;
  margin-top: -50px;
}

.title_slide {
    position: relative;
    text-align: center;

}

.title_slide h2 {
    color: var(--bleu);
    font-size: 35px;
    line-height: 42px;

    margin-top: -30px;
}

.title_slide img {
   text-align: center;
   width: 130px;
   transform: rotate(-31deg);
}

.slide_mobile {
    text-align: center;
}

.slide_mobile img {
    width: 200px;
    transform: rotate(26deg);
}

.slide_tiny {
  padding: 20px;
  margin-top: -60px;
}

.slide_tiny img {
  width: 100%;
  height: 400px;
  border-radius: 200px 200px 0 0;
  object-fit: cover;
}

.slide_tiny h3{
  color: var(--black);
  margin-top: 10px;
  font-size: 26px;
}

.btn_slide {
  text-align: center;
  margin: 30px 0 50px 0;
}

.btn_slide button{
    border: none;
  padding: 16px 58px;
  background-color: var(--orange);
  color: var(--white);
  font-size: 16px;
  position: relative;
}

.pic img {
  position: absolute; 
  left: -50px; 
  transform: rotate(180deg);
  bottom: -10px;
  z-index: 4;
}
</style>
