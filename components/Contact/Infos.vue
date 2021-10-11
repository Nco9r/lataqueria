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
       <div class="span_desktop">
        <hr />
        <hr />
      </div>
      <div class="item_infos">
        <div class="img">
          <img src="~assets/img/svg/phone.svg" alt="" />
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
       <div class="span_desktop">
        <hr />
        <hr />
      </div>
      <div class="item_infos">
        <div class="img">
          <img src="~assets/img/svg/food_court.svg" alt="" />
        </div>
        <div class="content">
          <h2>Boca Food Court</h2>
          <p>Quai de Paludate, BORDEAUX</p>
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

  .span_desktop {
    display: none;
  }

@media screen and (min-width: 1024px) {
  .infos {
    max-width: 1000px;
    margin: 50px auto;
  }



  .items {
    text-align: center;
    display: flex;
    flex-flow: row;
    width: 80%;
    justify-content: space-between;
    margin: 50px auto;
  }

  .item_infos .span {
    display: none;
  }

  .item_infos img {
    height: 60px;
  }

  .span_desktop {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  .span_desktop hr:nth-child(1) {
    width: 3px;
    background-color: var(--white);
    height: 120px;
    border: none;
    text-align: center;
    margin-right: 5px;
  }

  .span_desktop hr:nth-child(2) {
    width: 3px;
    background-color: var(--yellow);
    height: 120px;
    border: none;
    text-align: center;
    margin: 0px auto 0px auto;
  }
}

@media screen and (min-width: 1200px) {
  .infos {
    max-width: 1150px;
    margin: 20px auto;
  }

  .item_infos img {
    height: 80px;
  }

  .items {
    width: 90%;
  }

  .span_desktop hr:nth-child(1) {
    height: 140px;
  }

  .span_desktop hr:nth-child(2) {
    height: 140px;
  }

  .content h2 {
    font-size: 26px;
    margin-bottom: 5px;
  }

  .content p {
    font-size: 20px;
  }
}

@media screen and (min-width: 1440px) {
  .infos {
    max-width: 1300px;
    margin: 20px auto;
  }

  .item_infos img {
    height: 80px;
  }

  .items {
    width: 90%;
  }

  .span_desktop hr:nth-child(1) {
    height: 140px;
  }

  .span_desktop hr:nth-child(2) {
    height: 140px;
  }

  .content h2 {
    font-size: 26px;
    margin-bottom: 5px;
  }

  .content p {
    font-size: 20px;
  }
}

@media screen and (min-width: 1600px) {
  .infos {
    max-width: 1500px;
    margin: 20px auto 50px auto;
  }

}
</style>
