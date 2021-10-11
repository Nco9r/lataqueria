<template>
  <footer>
    <div class="box_footer">
    <div class="items_footer">
      <div class="item_logo">
        <img src="~assets/img/svg/Logo_taqueria.svg" alt="" />
        <p>
          Restauration convivial proposant de la street food mexicaine de
          qualité, dans le respect des recettes traditionnelles et 100% fait
          maison.
        </p>
      </div>
      <div class="item_footer">
        <div class="item">
          <h3>Sitemap</h3>
          <p>Accueil</p>
          <p>Menu</p>
          <p>Boutique</p>
          <p>Contact</p>
        </div>
        <div class="item">
          <h3>Legales</h3>
          <p>Politique de confidentialités</p>
          <p>Mentions Légales</p>
          <p>Cookies</p>
        </div>
         <div class="item">
          <h3>Sociaux</h3>
          
          <a href="https://www.facebook.com/lataqueriabordeaux/" target="_blank"><img src="~assets/img/svg/fb.svg" alt="" /></a>
         <a href="https://fr.linkedin.com/company/la-boca-foodcourt" target="_blank"><img src="~assets/img/svg/in.svg" alt="" /></a>
         <a href="https://www.instagram.com/lataqueriabordeaux/" target="_blank"><img src="~assets/img/svg/instagram.svg" alt="" /></a>
        </div>
      </div>
    </div>
    <div class="copyright">
        <p><span class="font">©2021 La taqueria</span>  - Charte graphique Noémie Pullido - Développement Nicolas ROUX</p>
    </div>
    </div>
    <div class="frise">
        <img src="~assets/img/svg/frise.svg" alt="">
    </div>
  </footer>
</template>

<script>
export default {}
</script>

<style scoped>
footer {
  z-index: 3;
  display: flex;
  flex-flow: column;
  overflow: hidden;
}


.items_footer {
  display: flex;
  padding: 20px;
  margin-top: 30px;
  flex-flow: column;
}

.item_logo img {
  width: 170px;
}

.item_logo p {
  width: 250px;
  font-size: 16px;
  margin-top: 20px;
  line-height: 22px;
}

.item_footer {
  display: flex;
  justify-content: space-between;
  margin-top: 50px;
  flex-flow: row wrap;
}

.item {
    width: 50%;
    margin-bottom: 40px;
}

.item h3 {
    font-size: 20px; 
    color: var(--orange);
    margin-bottom: 15px;
}

.item p {
    margin-bottom: 10px;
    font-size: 18px; 
    line-height: 22px;
}

.item img {
    margin-right: 20px;
}

.copyright {
    padding: 0px 20px 20px 20px;
    margin-top: -20px;
}

.copyright p {
    font-size: 16px; 
    line-height: 22Px;
}

.font {
    font-family: Barbaro, 'Times New Roman', Times, serif;
}

.frise {
    margin-bottom: -60px;
}

.frise img {
    width: 210%;
}

@media screen and (min-width: 1024px) {
    .items_footer {
        display: flex; 
        ;
        flex-flow: row wrap;
        justify-content: space-between;
    }

    .item_footer {
        width: 50%;
    }

    .item {
        width: 30%;
    }

    .frise img {
    width: 100%;
    margin-bottom: -80px;
}
}

@media screen and (min-width: 1200px) {
    footer {
        max-width: 1150px; 
        margin: auto;
    }
    .items_footer {
        display: flex; 
        ;
        flex-flow: row wrap;
        justify-content: space-between;
    }

    .item_footer {
        width: 50%;
    }


    .frise img {
    width: 100%;
    margin-bottom: -120px;
}

    .item {
        width: 25%;
    }
}

@media screen and (min-width: 1440px) {
    footer {
        max-width: 1500px; 
        margin: auto;
    }
    .items_footer {
        display: flex; 
        ;
        flex-flow: row wrap;
        justify-content: space-between;
    }

    .item_footer {
        width: 50%;
    }


    .frise img {
    width: 100%;
    margin-bottom: -80px;
}

    .item {
        width: 25%;
    }
}
</style>
