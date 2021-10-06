<template>
  <section class="slide">
    <div class="img_welcome">
      <img src="~assets/img/svg/pic.svg" alt="" />
    </div>
    <div class="title_slide">
      <img src="~assets/img/svg/sun.svg" alt="" />
      <h2>Mexican street food to BORDEAUX</h2>
    </div>
    <div class="slide_mobile">
      <img src="~assets/img/svg/tequila.svg" alt="" />
    </div>
    <client-only>
      <vue-tiny-slider v-bind="tinySliderOptions" ref="tinySlider">
        <div class="slide_box">
          <img src="~assets/img/png/quesadillas.jpg" alt="" />
          <h3>quesadillas</h3>
        </div>
        <div class="slide_box">
          <img src="~assets/img/png/BF.jpg" alt="" />
          <h3>Burrito Frites</h3>
        </div>
         <div class="slide_box">
          <img src="~assets/img/png/Tacos.jpg" alt="" />
          <h3>Tacos</h3>
        </div>
         <div class="slide_box">
          <img src="~assets/img/png/Tacos_2.jpg" alt="" />
          <h3>Tacos</h3>
        </div>
         <div class="slide_box">
          <img src="~assets/img/png/nachos.jpg" alt="" />
          <h3>Nachos</h3>
        </div>
         <div class="slide_box">
          <img src="~assets/img/png/BOWL.jpg" alt="" />
          <h3>Bowl Mex Frites</h3>
        </div>
         <div class="slide_box">
          <img src="~assets/img/png/Salade.jpg" alt="" />
          <h3>Salade Mex</h3>
        </div>
      </vue-tiny-slider>
    </client-only>
    <div class="slide_nav">
        <button class="slidePrev" id="prev">
            <img src="@/assets/img/svg/slide_arrow.svg" alt="" />
        </button>
         <button class="slideNext" id="next">
            <img src="@/assets/img/svg/slide_arrow.svg" alt="" />
        </button>
    </div>
    <div class="btn_slide">
      <button>Voir la Carte</button>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      tinySliderOptions: {
        mouseDrag: true,
        loop: true,
        items: 1,
        nav: false,
        gutter: 10,
        preventScrollOnTouch: 'auto',
        controls: true,
        prevButton: '#prev',
        nextButton: '#next',
        responsive: {
          1200: {
            items: 2,
          },
        },
      },
    }
  },
}
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
  display: block;
 ;
}

.tns-carousel{
    display: flex;
  flex-flow: row nowrap;
  justify-content: center;
}

.tns-item {
    margin-right: 20px;
    margin-top: -10px;
}

.slide_box {
  padding: 20px;
  display: block;
  margin-top: -70px;
  z-index: 2;
}

.slide_box img {
  width: 100%;
  height: 400px;
  border-radius: 200px 200px 0 0;
  object-fit: cover;
}

.slide_box h3 {
  color: var(--black);
  margin-top: 10px;
  width: 200px;
  font-size: 26px;
}

.slide_nav {
    display: flex;
    justify-content: center;
    margin-top: -10px;
}

.slide_nav button {
    border: none;
    background-color: transparent;
}

.slide_nav button:nth-child(1) {
    transform: rotate(180deg);
    margin-top: -6px;
    margin-right: 20px;
    pointer-events: all;
}

.btn_slide {
  text-align: center;
  margin: 30px 0 50px 0;
}

.btn_slide button {
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
