<template>
  <section class="menu">
    <div class="pic">
      <img src="~assets/img/svg/pic.svg" alt="" />
    </div>
    <div class="menu_hr">
      <hr />
      <div class="items_menu" @click="display = !display">
        <h2 v-if="plats">Nos plats</h2>
        <h2 v-if="partage">A partager</h2>
        <h2 v-if="plus">Boissons</h2>
        <img src="~assets/img/svg/select_orange.svg" alt="" />
      </div>
      <p class="offer" v-if="display">Découvrer égalements</p>
      <div class="items_menu_display" v-if="display">
        <h2
          @click="
            ;(partage = false),
              (plats = true),
              (plus = false),
              (display = !display)
          "
          v-if="!plats"
        >
          Nos plats
        </h2>
        <h2
          @click="
            ;(partage = true),
              (plats = false),
              (plus = false),
              (display = !display)
          "
          v-if="!partage"
        >
          a partager
        </h2>
        <h2  @click="
            ;(partage = false),
              (plats = false),
              (plus = true),
              (display = !display)
          "
          v-if="!plus">Boissons</h2>
      </div>
      <hr />
    </div>
    <div class="plats" v-if="plats">
      <div class="items_carte">
        <div class="infos_items">
          <h4>Tacos</h4>
          <h5>12,90</h5>
        </div>
        <div class="decriptif">
          <p>
            3 galettes de mais + Guacamole et crudités, garnitures aux choix.
          </p>
        </div>
      </div>
      <div class="items_carte">
        <div class="infos_items">
          <h4>Burritos</h4>
          <h5>12,90</h5>
        </div>
        <div class="decriptif">
          <p>
            Galettes de blé roulée, riz parfumé au citron vert et à la coriandre
            + Haricots noirs (ou frites), Guacamole, Cheddar, Mozzarella et
            crudités, Garnitures aux choix
          </p>
        </div>
      </div>
      <div class="items_carte">
        <div class="infos_items">
          <h4>quesadillas</h4>
          <h5>12,90</h5>
        </div>
        <div class="decriptif">
          <p>
            Galettes de blé grillé, poivrons grillés, cheddar, Mozzarella,
            Crudités. Garnitures au choix !
          </p>
        </div>
      </div>
      <div class="items_carte">
        <div class="infos_items">
          <h4>Bowl Mexicain</h4>
          <h5>12,90</h5>
        </div>
        <div class="decriptif">
          <p>
            Assiette de riz parfumé au citron vert et à la coriandre, Haricots
            noirs (ou frites), poivrons grillés et Guacamole. Garnitures au
            choix !
          </p>
        </div>
      </div>
      <div class="items_carte">
        <div class="infos_items">
          <h4>Salade Mexicaine</h4>
          <h5>12,90</h5>
        </div>
        <div class="decriptif">
          <p>
            Assiette de salade Avocat, Tomates, Mais, Radis, Fêta, Oignons,
            Vinaigrette au citron Vert. Poulet ou filet de thon au choix.
          </p>
        </div>
      </div>
        <div class="items_carte">
        <div class="infos_items">
          <h4>Dessert du jour</h4>
          <h5>5</h5>
        </div>
        <div class="decriptif">
          <p>
            Dessert du chef en fonction des saisons.
          </p>
        </div>
      </div>
    </div>

    <div class="partage" v-if="partage">
      <div class="items_carte">
        <div class="infos_items">
          <h4>Nachos et Guacamole</h4>
          <h5>7</h5>
        </div>
      </div>
      <div class="items_carte">
        <div class="infos_items">
          <h4>Maxi Plateau 3/4 pers</h4>
          <h5>26</h5>
        </div>
        <div class="decriptif">
          <p>4 Quesadillas, 3 Tacos, Nachos et Guacamole.</p>
        </div>
      </div>
       <div class="items_carte">
        <div class="infos_items">
          <h4>En portion</h4>
          <h5>3,90</h5>
        </div>
        <div class="decriptif">
          <p>Frites, Riz/Haricots, Crudités, Nachos + Guacamole.</p>
        </div>
      </div>
    </div>

     <div class="plus" v-if="plus">
        <div class="items_carte">
        <div class="infos_items">
          <h4>Abatilles Plate</h4>
          <h5>2</h5>
        </div>
        <div class="decriptif">
          <p>Bouteille 50cl</p>
        </div>
      </div>
       <div class="items_carte">
        <div class="infos_items">
          <h4>Abatilles Petillante</h4>
          <h5>3</h5>
        </div>
        <div class="decriptif">
          <p>Bouteille 50cl</p>
        </div>
      </div>
      <div class="items_carte">
        <div class="infos_items">
          <h4>Perrier Ananas Mangue</h4>
          <h5>3</h5>
        </div>
        <div class="decriptif">
          <p>Eau gazeuse arômes ananas et mangue</p>
        </div>
      </div>
      <div class="items_carte">
        <div class="infos_items">
          <h4>Coca</h4>
          <h5>3</h5>
        </div>
        <div class="decriptif">
          <p>Canette 33 cL</p>
        </div>
      </div>
       <div class="items_carte">
        <div class="infos_items">
          <h4>Coca zero</h4>
          <h5>3</h5>
        </div>
        <div class="decriptif">
          <p>Canette 33 cL</p>
        </div>
      </div>
      <div class="items_carte">
        <div class="infos_items">
          <h4>Jarritos Ananas</h4>
          <h5>4,50</h5>
        </div>
        <div class="decriptif">
          <p>Soda typique mexicain saveur citron</p>
        </div>
      </div>
      <div class="items_carte">
        <div class="infos_items">
          <h4>Jarritos mangue</h4>
          <h5>4.5</h5>
        </div>
        <div class="decriptif">
          <p>Soda typique mexicain saveur Mangue</p>
        </div>
      </div>
      <div class="items_carte">
        <div class="infos_items">
          <h4>Jarritos goyave</h4>
          <h5>4.5</h5>
        </div>
        <div class="decriptif">
          <p>Soda typique mexicain saveur Goyave</p>
        </div>
      </div>
      <div class="items_carte">
        <div class="infos_items">
          <h4>Jarritos Mandarine</h4>
          <h5>4.5</h5>
        </div>
        <div class="decriptif">
          <p>Soda typique mexicain saveur Mandarine</p>
        </div>
      </div>
      <div class="items_carte">
        <div class="infos_items">
          <h4>Jarritos Pamplemousse Vert</h4>
          <h5>4.5</h5>
        </div>
        <div class="decriptif">
          <p>Soda typique mexicain saveur Pamplemousse Vert</p>
        </div>
      </div>
      <div class="items_carte">
        <div class="infos_items">
          <h4>Desperados</h4>
          <h5>6</h5>
        </div>
        <div class="decriptif">
          <p>Bière blonde aromatisée à la tequila</p>
        </div>
      </div>
      <div class="items_carte">
        <div class="infos_items">
          <h4>Corona</h4>
          <h5>6</h5>
        </div>
        <div class="decriptif">
          <p>Bière lager mexicaine</p>
        </div>
      </div><div class="items_carte">
        <div class="infos_items">
          <h4>Nacion Lager - Nacional</h4>
          <h5>6</h5>
        </div>
        <div class="decriptif">
          <p>Bière lager artisanale mexicaine</p>
        </div>
      </div><div class="items_carte">
        <div class="infos_items">
          <h4>Siervo - Nacional</h4>
          <h5>6</h5>
        </div>
        <div class="decriptif">
          <p>Bière blanche artisanale mexicaine</p>
        </div>
      </div>
      <div class="items_carte">
        <div class="infos_items">
          <h4>El Conquistador</h4>
          <h5>6</h5>
        </div>
        <div class="decriptif">
          <p>Bière lager mexicaine</p>
        </div>
      </div>
       <div class="items_carte">
        <div class="infos_items">
          <h4>La Muerte - Blanche</h4>
          <h5>6</h5>
        </div>
        <div class="decriptif">
          <p>Bière blanche mexicaine</p>
        </div>
      </div>
     </div>



    <div class="price">
      <p>Tous nos prix sont affcihés en euros et TTC.</p>
      <p>L'abus d'alcool est dangereux pour la santé. À consommer avec modération.</p>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      display: false,
      plats: true,
      partage: false,
      plus: false,
    }
  },
}
</script>

<style scoped>
.menu {
  background-color: var(--white);
  margin-top: -200px;
  padding-bottom: 50px;
  background-image: url('assets/img/svg/bck.svg');
  background-repeat: repeat;
  background-size: 250%;
}

.pic {
  overflow-x: hidden;
  padding-top: -50px;
  z-index: 10;
}

.menu_hr {
  margin: 220px 20px 20px 20px;
  position: sticky;
  background-color: var(--white);
  top: 100px;
}

.menu_hr hr {
  background-color: var(--black);
  border: none;
  height: 1px;
}

.items_menu {
  color: var(--orange);
  margin-top: 20px;
  display: flex;
  padding: 0 20px;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}

.items_menu h2 {
  font-size: 28px;
  -webkit-text-stroke: 1px var(--orange);
  color: transparent;
}

.offer {
  color: var(--black);
  padding: 0 20px;
  margin-top: -10px;
  margin-bottom: 10px;
  font-weight: bold;
}

.items_menu_display {
  display: flex;
  padding: 0 20px;
}

.items_menu_display h2 {
  color: var(--orange);
  font-size: 20px;
  margin-right: 20px;
  margin-bottom: 20px;
}

.items_carte {
  padding: 15px 25px;
  display: flex;
  flex-flow: column;
}

.infos_items {
  display: flex;
  flex-flow: row;
  justify-content: space-between;
  align-items: flex-end;
}

.infos_items h5 {
  color: var(--black);
  font-size: 18px;
}
.infos_items span {
  /* background-color: var(--black); */
  height: 0.1px;
  width: 100%;
  margin: 0px 20px 5px 20px;
}
.infos_items h4 {
  color: var(--black);
  font-size: 18px;
}

.decriptif p {
  color: var(--orange);
  margin-top: 5px;
  font-family: ColabMed, sans-serif;
  line-height: 20px;
  font-size: 14px;
}

.price {
  display: flex;
  justify-content: flex-end;
  flex-flow: column;
  padding: 10px 25px 0px 25px;
}

.price p{
  color: var(--semi-gray);
  margin-bottom: 5px;
}
</style>
