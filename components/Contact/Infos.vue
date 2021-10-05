<template>
  <section class="infos">
    <div class="items">
      <div class="item_infos">
        <div class="img">
          <img src="~assets/img/svg/email.svg" alt="" />
        </div>
        <div class="content">
          <h2>Email</h2>
          <p>tacos@lataqueria-bordeaux.fr</p>
        </div>
        <div class="span">
          <hr />
          <hr />
        </div>
      </div>
      <div class="item_infos">
        <div class="img">
          <img src="~assets/img/svg/clock.svg" alt="" />
        </div>
        <div class="content">
          <h2>Téléphone</h2>
          <p>07 54 82 76 76</p>
        </div>
        <div class="span">
          <hr />
          <hr />
        </div>
      </div>
      <div class="item_infos">
        <div class="img">
          <img src="~assets/img/svg/delivreoo.svg" alt="" />
        </div>
        <div class="content">
          <h2>livraison</h2>
          <p>Faites vous livrer</p>
        </div>
      </div>
    </div>
    <div class="hr_infos">
        <hr>
        <hr>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style scoped>
.infos {
  text-align: center;
  display: flex;
  flex-flow: column;
  margin-top: 50px;
}

.content h2 {
  font-weight: 500;
}

.item_infos img {
  margin-bottom: 20px;
}

.span {
  width: 200px;
  height: 10px;
  margin: 60px auto;
}

.span hr:nth-child(1) {
  width: 100%;
  background-color: var(--white);
  height: 3px;
  border: none;
  text-align: center;
  margin: 30px auto 5px auto;
}

.span hr:nth-child(2) {
  width: 100%;
  background-color: var(--yellow);
  height: 3px;
  border: none;
  text-align: center;
  margin: 0px auto 30px auto;
}

.hr_infos hr:nth-child(1) {
    width: 90%;
  background-color: var(--white);
  height: 3px;
  border: none;
  text-align: center;
  margin: 60px auto 5px auto;
}

.hr_infos hr:nth-child(2) {
    width: 90%;
  background-color: var(--white);
  height: 3px;
  border: none;
  text-align: center;
  margin: 0px auto 60px auto;
}

</style>
