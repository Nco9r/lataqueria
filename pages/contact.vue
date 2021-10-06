<template>
  <main>
    <div class="open">
      <div class="text">
        <img src="~assets/img/svg/tacos_cursor.svg" alt="">
      </div>
    </div>
    <Hero />
    <infos/>
    <Form/>
  </main>
</template>

<script>
import Hero from '../components/Contact/Hero'
import Infos from '../components/Contact/Infos'
import Form from '../components/Contact/Form'
export default {
  components: {
    Hero,
    Infos,
    Form
  },
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
</style>
