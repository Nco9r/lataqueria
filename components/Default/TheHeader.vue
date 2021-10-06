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
        <div class="item_header">
          <nuxt-link to="/">Accueil</nuxt-link>
          <nuxt-link to="/menu">Menu</nuxt-link>
          <nuxt-link to="/">Boutique</nuxt-link>
          <button>Contact</button>
        </div>
        <div class="item_sociaux">
          <img src="~assets/img/svg/fb.svg" alt="" />
          <img src="~assets/img/svg/in.svg" alt="" />
          <img src="~assets/img/svg/instagram.svg" alt="" />
           <p>
            ©2021 <span class="font">La taqueria</span> - Charte graphique Noémie Pullido - Développement
            Nicolas ROUX
          </p>
        </div>
      </div>
    </transition>
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


</style>
