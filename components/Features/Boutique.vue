<template>
  <section class="boutique">
    <div class="top_img">
      <div class="img">
        <img src="~assets/img/svg/sun_2.svg" alt="" />
        <img src="~assets/img/svg/sun_2.svg" alt="" />
        <img src="~assets/img/svg/extra_1.svg" alt="" />
      </div>
    </div>
    <div class="store">
      <div class="content_store">
        <div class="title_store">
          <h2>Commandez nos produits pour vos soirées</h2>
          <p>
            Vous organisez une soirée mexicain ? Vous pouvez directement
            commander nos produits dans notre boutique et épater vos convives
            avec des produits authentiques Mexicain !
          </p>
        </div>
      </div>
      <div class="product_store">
        <div class="item_product">
          <div class="img_product">
            <img src="~assets/img/png/product.png" alt="" />
            <img src="~assets/img/svg/boutique.svg" alt="" />
            <!-- <div class="add">
              <img src="~assets/img/svg/star.svg" alt="" />
              <p>+</p>
            </div> -->
          </div>
          <div class="title_product">
            <h3>Tortillas Chips</h3>
          </div>
          <div class="details">
            <div class="description_details">
              <p>BBQ PAPRIKA | Les 150g</p>
            </div>
            <div class="price">
              <p>3,90€</p>
            </div>
          </div>
        </div>
         <div class="item_product">
          <div class="img_product">
            <img src="~assets/img/png/product.png" alt="" />
            <img src="~assets/img/svg/boutique.svg" alt="" />
            <!-- <div class="add">
              <img src="~assets/img/svg/star.svg" alt="" />
              <p>+</p>
            </div> -->
          </div>
          <div class="title_product">
            <h3>Tortillas Chips</h3>
          </div>
          <div class="details">
            <div class="description_details">
              <p>BBQ PAPRIKA | Les 150g</p>
            </div>
            <div class="price">
              <p>3,90€</p>
            </div>
          </div>
        </div>
         <div class="item_product">
          <div class="img_product">
            <img src="~assets/img/png/product.png" alt="" />
            <img src="~assets/img/svg/boutique.svg" alt="" />
            <!-- <div class="add">
              <img src="~assets/img/svg/star.svg" alt="" />
              <p>+</p>
            </div> -->
          </div>
          <div class="title_product">
            <h3>Tortillas Chips</h3>
          </div>
          <div class="details">
            <div class="description_details">
              <p>BBQ PAPRIKA | Les 150g</p>
            </div>
            <div class="price">
              <p>3,90€</p>
            </div>
          </div>
        </div>
      </div>
      <div class="btn_store">
        <button>Boutique</button>
      </div>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style scoped>
.boutique {
  margin-top: 30px;
}
.top_img {
  width: 100%;
  position: relative;
  height: 500px;
  background-image: url('~assets/img/png/store_1.jpg');
  background-size: 120%;
  background-repeat: no-repeat;
  background-position: 100% 10%;
}

.img img:nth-child(1) {
  width: 50px;
  position: absolute;
  top: 30px;
  transform: rotate(-120deg);
  left: 10px;
}

.img img:nth-child(2) {
  width: 50px;
  position: absolute;
  top: 30px;
  right: 10px;
}

.img img:nth-child(3) {
  width: 320px;
  position: absolute;
  bottom: 120px;
  left: 5%;
}

.store {
  background-color: var(--orange);
  width: 100%;
  margin-top: -180px;
  z-index: -1;
  padding-bottom: 50px;
  background-image: url('assets/img/svg/head.svg');
  background-repeat: no-repeat;
  background-size: 300%;
  background-position: 50%;
}

.content_store {
  padding: 80px 5px 30px 5px;
  text-align: center;
}
.title_store h2 {
  font-size: 35px;
  line-height: 40px;
  font-weight: 500;
}

.title_store p {
  font-size: 16px;
  line-height: 22px;
  width: 358px;
  margin: 10px auto;
}

.product_store {
  display: flex;
  flex-flow: column;
  align-items: center;
  justify-content: center;
}

.item_product {
  margin-bottom: 80px;
}

.item_product .img_product img {
  width: 230px;
}

.img_product {
  display: flex;
  flex-flow: column;
}

.img_product img:nth-child(1) {
  z-index: 1;
}
.img_product img:nth-child(2) {
  margin-top: -70px;
  z-index: 0;
}

.add {
  position: absolute;
  z-index: 2;
  display: flex;
  justify-content: center;
  align-items: center;
  right: 70px;
}

.add p {
  background-color: var(--orange);
  width: 30px;
  position: absolute;
  z-index: 2;
  display: flex;
  justify-content: center;
  align-items: center;
  right: 45px;
  top: 38px;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 30px;
  font-size: 14px;
  border-radius: 50%;
}

.add img {
  width: 120px !important;
}

.title_product {
  margin-top: 10px;
  margin-left: 10px;
  font-size: 18px;
}

.description_details {
  margin-left: 10px;
}

.details {
  display: flex;
  flex-flow: row;
  align-items: flex-end;
  justify-content: space-between;
}

.price p {
  color: var(--black);
  font-family: Barbaro, sans-serif;
  font-size: 24px;
}

.btn_store {
  text-align: center;
}

.btn_store button{
    border: none;
  padding: 16px 58px;
  background-color: var(--yellow);
  color: var(--black);
  font-size: 16px;
  position: relative;
}
</style>
