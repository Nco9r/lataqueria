<template>
  <div class="cookies" v-if="valideCookie">
    <div class="content_cookies">
      <div class="content">
        <img src="~assets/img/svg/cookie.svg" alt="" />
        <p>
          Nous utilisons des cookies tiers pour personnaliser le contenu, les
          publicités et analyser le trafic du site. <strong><nuxt-link to="/"> savoir plus</nuxt-link></strong>
        </p>
        <button @click="valide">Accepter</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      valideCookie: false,
    }
  },
  mounted() {
    const cookies = this.$cookies.get('Cookies_Taqueria')
    this.valideCookie = cookies === undefined
  },
  methods: {
    valide() {
      this.valideCookie = !this.valideCookie
      this.$cookies.set('Cookies_Taqueria', true, {
        path: '/',
        maxAge: 60 * 60 * 24 * 365,
      })
    },
  },
}
</script>

<style scoped>
a {
    font-size: 14px;
    color: var(--black);
}

.cookies {
  position: fixed;
  background-color: var(--white);
  bottom: 20px;
  background-image: url('assets/img/svg/bck.svg');
  background-repeat: repeat;
  background-size: 150%;
  height: 230px;
  z-index: 9;
  left: 20px;
  border-radius: 3px;
  box-shadow: 0 12px 12px -10px rgba(37, 37, 37, 0.74);

  right: 20px;
}

.content_cookies {
  display: flex;
  flex-flow: column;
  padding: 25px;
  justify-content: center;
  align-items: center;
  text-align: center;
  color: var(--black);
}

.content img {
    width: 40px;
    margin-bottom: 15px;
}

.content p {
  color: var(--black);
  line-height: 20px;
  margin-bottom: 15px;
}

.content button {
     border: none;
  padding: 10px 38px;
  background-color: var(--orange);
  color: var(--white);
  font-size: 14px;
  position: relative;
}
</style>
