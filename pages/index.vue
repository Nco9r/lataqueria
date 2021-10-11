<template>
  <main>
    <div class="open">
      <div class="text">
        <img src="~assets/img/svg/tacos_cursor.svg" alt="">
      </div>
    </div>
    <Hero />
    <Infos/>
    <Concept/>
    <Boutique/>
    <Slide/>
    <!-- <div class="button" @click="scrollTop">
      <p>Top</p>
    </div> -->
  </main>
</template>

<script>
import Boutique from '../components/Features/Boutique.vue'
import Concept from '../components/Features/Concept.vue'
import Hero from '../components/Features/Hero.vue'
import Infos from '../components/Features/Infos.vue'
import Slide from '../components/Features/Slide.vue'
export default {
  components: {
    Hero,
    Infos,
    Concept,
    Boutique,
    Slide
  },
  methods: {
    scrollTop() {
      window.scrollTo({
        top: 0,
        behavior: 'smooth'
      })
    }
  }
}
</script>

<style>

.open {
  position: fixed;
  top: 0;
  background-color: var(--bleu);
  width: 100%;
  height: 100vh;
  background-image: url('assets/img/svg/bck.svg');
  background-repeat: repeat;
  background-size: 150%;
  overflow: hidden;
  z-index: 1000;
  animation: open 0.5s linear;
  animation-delay: 1.3s;
  animation-fill-mode: forwards;
}

@keyframes open {
  from {
    top: 0;
  }
  to {
    top: -120%;
  }
}

@keyframes appear {
  from {
    opacity: 0;
    transform: translateY(30px);
  } to {
    opacity: 1;
    transform: translateY(0px);
  }
}

.text {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-flow: column;
  height: 100vh;
  
}

.text  img{

width: 50px;
opacity: 0;
animation: appear 1s linear;
  animation-delay: .3s;
  animation-fill-mode: forwards;
margin-left: -20px;

}


.button {
  position: fixed;
  bottom: 10px;
  right: 10px;
  background-color: var(--orange);
  width: 50px;
  font-weight: bold;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 50px;
  border-radius: 50%;
  z-index: 1;
}

@media screen and (min-width: 1024px) {
  .open {
     background-image: url('assets/img/svg/bck.svg');
  background-repeat: repeat;
  background-size: 50%;
  }
}

</style>