<template>
  <section class="form">
    <div class="sun">
      <img src="~assets/img/svg/sun_2.svg" alt="" />
      <img src="~assets/img/svg/sun_2.svg" alt="" />
    </div>
    <form>
      <div class="form_group">
        <div class="label_form">
          <div class="label">
            <h2>Votre Nom</h2>
          </div>
          <div class="input">
            <input type="text" required placeholder="El Gordo" />
          </div>
        </div>
        <div class="label_form">
          <div class="label">
            <h2>Votre Email</h2>
          </div>
          <div class="input">
            <input type="email" required placeholder="votre@email.fr" />
          </div>
        </div>
        <div class="label_form">
          <div class="label">
            <h2>Votre Télephone</h2>
          </div>
          <div class="input">
            <input type="tel" required placeholder="06 ** ** ** **" />
          </div>
        </div>
        <div class="label_form">
          <div class="label">
            <h2>Votre Demande</h2>
          </div>
          <div class="input">
            <select name="" id="">
              <option value="liste" selected disabled>
                Selectionnez un choix
              </option>
              <option value="bonjour">Bonjour :)</option>
              <option value="groupe">Repas de groupe</option>
              <option value="boutique">Boutique</option>
            </select>
          </div>
        </div>
        <div class="label_form">
          <div class="label">
            <h2>Votre Message</h2>
          </div>
          <div class="input">
            <textarea
              type="text"
              rows="15"
              required
              placeholder="Miam les bons tacos !"
            ></textarea>
          </div>
        </div>
        <div class="label_check">
          <input type="checkbox" required />
          <p>
            En complétant ce formulaire vous consentez à ce que La Taqueria
            traite vos données personnelles. Pour en savoir plus sur la gestion
            de vos données personnelles par La Taqueria vous pouvez vous
            reporter au mentions légales.
          </p>
        </div>
        <div class="btn_form">
          <button>Soumettre votre demande</button>
        </div>
      </div>
    </form>
  </section>
</template>

<script>
export default {}
</script>

<style scoped>
.form {
  background-color: var(--white);
  background-image: url('assets/img/svg/bck.svg');
  background-repeat: repeat;
  background-size: 250%;
  position: relative;
}

.sun img:nth-child(1) {
  width: 60px;
  position: absolute;
  top: 10px;
  transform: rotate(-120deg);
  left: 20px;
}

.sun img:nth-child(2) {
  width: 60px;
  position: absolute;
  top: 10px;
  right: 20px;
}

form {
  padding: 120px 20px 50px 20px;
}

.label_form {
  margin-bottom: 25px;
}

.label h2 {
  color: var(--orange);
  font-size: 16px;
  margin-left: 5px;
  margin-bottom: 7px;
}

.label h2::after {
  content: '*';
  margin-left: 3px;
}

.input input {
  border: 1px solid var(--gray);
  padding: 18px 24px;
  outline: none;
  color: var(--black);
  font-size: 16px;
  -webkit-appearance: none;
  border-radius: 0;
  width: 100%;
}

.input select {
  background-color: var(--orange);
  padding: 18px 24px;
  outline: none;
  font-size: 16px;
  -webkit-appearance: none;
  border: none;
  border-radius: 0;
  color: var(--white);
  font-weight: bold;
  background-image: url('~assets/img/svg/select.svg');
  background-repeat: no-repeat;
  background-position: 95% 50%;
  width: 100%;
}

.input textarea {
  border: 1px solid var(--gray);
  padding: 18px 24px;
  outline: none;
  font-size: 16px;
  width: 100%;
  color: var(--black);

  -webkit-appearance: none;
  border-radius: 0;
}

.input textarea::placeholder {
  color: var(--gray);
}

.input input::placeholder {
  color: var(--gray);
}

.label_check {
  display: flex;
  align-items: flex-start;
}

.label_check p {
  color: var(--semi-gray);
  margin-left: 20px;
  line-height: 20px;
}

input[type='checkbox' i] {
  background-color: var(--white) !important;
  width: 90px;
  height: 25px;
  border: 1px solid var(--gray);
  border-radius: 0px;
  -webkit-appearance: none;
  outline: none;
  transition: all 0.3s;
}

input[type='checkbox' i]:checked {
  background-color: var(--orange) !important;
  width: 90px;
  height: 25px;
  -webkit-appearance: none;
  display: flex;
  transition: all 0.3s;
}

input[type='checkbox' i]:checked::after {
  content: 'x';
  font-size: 16px;
  color: white;
  font-weight: bold;
  display: flex;
  margin: auto;
}

.btn_form {
  margin-top: 30px;
}

.btn_form button {
  border: none;
  padding: 16px;
  width: 100%;
  background-color: var(--orange);
  color: var(--white);
  font-size: 16px;
  position: relative;
}
</style>
