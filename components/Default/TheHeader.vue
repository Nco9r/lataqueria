<template>
  <header>
    <div class="header_mobile">
      <div class="logo_header">
        <img src="~assets/img/svg/Logo_taqueria.svg" alt="" />
      </div>
      <div class="items_header">
        <div class="cart_header">
          <img src="~assets/img/svg/cart.svg" alt="" />
        </div>
        <hr class="hr_header" />
        <tasty-burger-button
          :type="buttonType"
          :active="isActive"
          :size="size"
          :color="color"
          :active-color="activeColor"
          v-on:toggle="onToggle"
        />
        <!-- <div class="hamburger_header">
         
          <span :class="{ open: close }"></span> -->
      </div>
    </div>
    <transition name="openMenu" appear>
      <div class="open_header" v-if="open">
        <div class="item_header" @click="onToggle">
          <nuxt-link to="/" @click="onToggle">Accueil</nuxt-link>
          <nuxt-link to="/menu" @click="onToggle">Menu</nuxt-link>
          <nuxt-link to="/boutique" @click="onToggle">Boutique</nuxt-link>
          <nuxt-link to="/contact" @click="onToggle">
            <button>Contact</button>
          </nuxt-link>
        </div>
        <div class="item_sociaux">
          <a href="https://www.facebook.com/lataqueriabordeaux/" target="_blank"
            ><img src="~assets/img/svg/fb.svg" alt=""
          /></a>
          <a
            href="https://fr.linkedin.com/company/la-boca-foodcourt"
            target="_blank"
            ><img src="~assets/img/svg/in.svg" alt=""
          /></a>
          <a
            href="https://www.instagram.com/lataqueriabordeaux/"
            target="_blank"
            ><img src="~assets/img/svg/instagram.svg" alt=""
          /></a>
          <p>
            ©2021 <span class="font">La taqueria</span> - Charte graphique
            Noémie Pullido - Développement Nicolas ROUX
          </p>
        </div>
      </div>
    </transition>
    <div class="header_desktop">
      <div class="box_header">
        <div class="header_desktop_logo">
          <img src="~assets/img/svg/Logo_taqueria.svg" alt="" />
        </div>
        <div class="header_desktop_items">
          <nuxt-link to="/" @click="onToggle">Accueil</nuxt-link>
          <nuxt-link to="/menu" @click="onToggle">Menu</nuxt-link>
          <nuxt-link to="/boutique" @click="onToggle">Boutique</nuxt-link>
          <img src="~assets/img/svg/cart.svg" alt="" />
            <span class="hr_header_desktop"></span>
          <nuxt-link to="/contact" @click="onToggle">
            <button>Contact</button>
          </nuxt-link>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  data() {
    return {
      open: false,
      buttonType: 'spin',
      isActive: false,
      size: 's',
      color: 'white',
      activeColor: '#EA6527',
    }
  },
  methods: {
    onToggle() {
      this.open = !this.open
    },
  },
}
</script>

<style scoped>
.header_mobile {
  display: flex;
  flex-flow: row;
  align-items: center;
  justify-content: space-between;
  padding: 20px 20px 0 20px;
  background-color: var(--bleu);
  position: fixed;
  left: 0;
  z-index: 10;
  right: 0;
  top: 0;
}

.logo_header {
  z-index: 3;
}

.logo_header img {
  width: 130px;
}

.items_header {
  display: flex;
  flex-flow: row;
  align-items: center;
  justify-content: space-between;
  z-index: 2;
}

.hr_header {
  border: none;
  width: 2px;
  height: 20px;
  background-color: var(--orange);
  margin-left: 20px;
  margin-right: 20px;
}

.hamburger_header {
  display: flex;
  flex-flow: column;
  width: 30px;
}

.hamburger-inner {
  width: 30px !important;
  height: 3px !important;
}

.hamburger:hover {
  opacity: 1 !important;
}

.hamburger-inner__before {
  width: 30px !important;
  height: 3px !important;
}

.hamburger-inner__after {
  width: 30px !important;
  height: 3px !important;
}

.open_header {
  position: fixed;
  inset: 0;
  background-color: var(--bleu);
  background-image: url('~assets/img/svg/head.svg');
  background-size: 100%;
  z-index: 2;
  background-position: 100% 50%;
  background-repeat: no-repeat;
}

@keyframes open {
  from {
    transform: translateX(100%);
  }
  to {
    transform: translateX(0);
  }
}

@keyframes close {
  from {
    transform: translateX(0);
  }
  to {
    transform: translateX(100%);
  }
}

.openMenu-enter-active {
  animation: open 0.5;
}

.opennMenu-leave-active {
  animation: close 0.5;
}

.item_header {
  display: flex;
  flex-flow: column;
  justify-content: center;
  align-items: center;
  margin-top: 35%;
}

.item_header a {
  font-family: Barbaro, 'Times New Roman', Times, serif;
  color: var(--white);
  text-decoration: none;
  margin-bottom: 50px;
  font-size: 42px;
}

.item_header button {
  border: none;
  padding: 16px 58px;
  background-color: var(--orange);
  color: var(--white);
  font-size: 20px;
  position: relative;
}

.item_sociaux {
  position: absolute;
  bottom: 10px;
  right: 20px;
  left: 20px;
}

.item_sociaux img {
  margin-right: 20px;
}

.item_sociaux p {
  margin-top: 10px;
  font-size: 14px;
  line-height: 20px;
}

.font {
  font-family: Barbaro, 'Times New Roman', Times, serif;
}

.header_desktop {
  display: none;
}

@media screen and (min-width: 1024px) {
  .header_desktop {
    display: flex;
    background-color: var(--bleu);
    position: fixed;
    left: 0;
    z-index: 10;
    right: 0;
    top: 0;
  }

  .header_mobile {
    display: none;
  }

  .box_header {
    max-width: 1000px !important;
    margin: 20px auto;
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .header_desktop_logo img {
    width: 120px;
    margin-left: 20px;
  }

  .header_desktop_items {
    display: flex;
    align-items: center;
  }

  .header_desktop_items a {
    font-family: Barbaro, sans-serif;
    font-size: 20px;
    margin-right: 50px;

    text-decoration: none;
    color: var(--white);
  }

  .header_desktop_items a button {
    border: none;
    padding: 12px 38px;
    background-color: var(--orange);
    color: var(--white);
    font-size: 20px;
    position: relative;
  }

  .hr_header_desktop {
     border: none;
  width: 2px;
  height: 20px;
  background-color: var(--orange);
  margin-left: 50px;
  margin-right: 50px;
  }
}

@media screen and (min-width: 1200px) {
  .box_header {
    max-width: 1200px !important;
    margin: 20px auto;
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
}

@media screen and (min-width: 1440px) {
  .box_header {
    max-width: 1400px !important;
    margin: 20px auto;
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
}

@media screen and (min-width: 1600px) {
  .box_header {
    max-width: 1600px !important;
    margin: 20px auto;
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
}
</style>
