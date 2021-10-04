<template>
  <section class="slide">
    <div class="img_welcome">
      <img src="~assets/img/svg/welcome.svg" alt="" />
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
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style scoped>
.slide {
  height: 500px;
  background-color: var(--white);
  background-image: url('assets/img/svg/bck.svg');
  background-repeat: repeat;
  background-size: 250%;
  overflow-x: hidden;
}



.img_welcome img {
  width: 200px;
  margin-left: 200px;
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
    width: 150px;
    transform: rotate(23deg);
}
</style>
