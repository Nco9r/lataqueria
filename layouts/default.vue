 <template>
  <div> 
    <the-header/>
    <cookies/>
    <nuxt/>
    <the-footer/>
  </div>
</template>

<script>

import TheHeader from '../components/Default/TheHeader.vue'
import TheFooter from '../components/Default/TheFooter.vue'
import Cookies from '../components/Default/Cookies.vue'
import VueLerpElement from "vue-lerp-element";

export default {
  components: {
    TheHeader,
    TheFooter,
    Cookies,
    VueLerpElement,
  }
}
</script>

<style>
html {
  font-family: 'RobotoMono', Times, serif;
  font-weight: 500;
  font-style: normal;
  font-size: 14px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  background-image: url('assets/img/svg/bck.svg');
  background-repeat: repeat;
  background-size: 250%;
  background-color: var(--bleu);
  color:var(--white);
  /* cursor: url('~assets/img/svg/tacos_cursor.svg'), auto; */

}



*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

:root {
  --black: #202020;
  --yellow: #F8E813;
  --orange: #EA6527;
  --bleu: #233F93;
  --white: #FFF;
  --gray: #D9D9D9;
  --semi-gray: rgb(82, 82, 82);
  --input: rgba(247, 247, 247, 0.20);
}

h1, h2, h3, h4, h5 {
  font-family: Barbaro, 'Times New Roman', Times, serif;
  letter-spacing: -.5px;
}

p {
  font-family: ColabLig, 'Times New Roman', Times, serif;
  color: var(--white);
}

button {
    font-family: Barbaro, 'Times New Roman', Times, serif;

}

input, textarea {
  font-family: ColabLig;
}






@font-face {
  font-family: Barbaro;
  src: url('~assets/fonts/barbaro_punta.ttf');
}

@font-face {
  font-family: ColabMed;
  src: url('~assets/fonts/ColabMed.ttf');
}

@font-face {
  font-family: ColabLig;
  src: url('~assets/fonts/ColabLig.ttf');
}



@media screen and (min-width: 1024px) {
  html {
    background-image: url('assets/img/svg/bck.svg');
  background-repeat: repeat;
  background-size: 80%;
  background-color: var(--bleu);
  }
}



</style>
