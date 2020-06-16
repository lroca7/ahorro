<template>
  <section class="resume">
    <div class="header">
      <div class="header__title">
        <p class="header__title--welcome">Hola, Camila</p>
        <div class="icon__container">
          <img
            class="icon"
            src="https://img.icons8.com/carbon-copy/100/000000/bell.png"
          />
        </div>
      </div>
    </div>
    <div class="invest__card">
      <div class="invest__motivation">
        <h3>Eres</h3>
        <h3>estratega</h3>
      </div>
      <h4>Tu Saldo</h4>
      <h1>$1.570.000</h1>
    </div>
    <div class="invest__summary">
      <div>
        <p>Inversión</p>
        <p>Rendimiento</p>
      </div>
      <div class="invest__summary--values">
        <p class="bold-600">$1.600.000</p>
        <p class="bold-600">-30.000</p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Resume",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
.invest__summary--values {
  font-weight: 600;
  text-align: end;
}

.invest__summary {
  display: flex;
  justify-content: space-between;
  align-items: center;
  color: #58506b;
  font-size: 14px;
  padding: 20px;
  margin-top: 5%;
  background: #ffffff;
  box-shadow: 0px 8px 20px rgba(197, 166, 236, 0.05);
  border-radius: 20px;
}

.invest__card {
  background: linear-gradient(
      180deg,
      rgba(44, 82, 216, 0) 0%,
      rgba(44, 82, 216, 0.4) 100%
    ),
    #54d1ed;
  background-blend-mode: multiply, normal;

  box-shadow: 0px 8px 20px rgba(197, 166, 236, 0.05);
  border-radius: 20px;

  color: #ffffff;
  font-weight: 600;
  font-size: 36px;
  line-height: 49px;

  padding: 30px;

  margin-top: 5%;
}

.invest__card img {
  position: absolute;
  height: 250px;
  right: 0px;
  top: 2%;
  left: 28%;
}

.invest__card h3 {
  margin: 0;
}

.invest__card h4 {
  line-height: 21px;
  margin: 0;
  font-size: 14px;
  margin-top: 90px;
}

.invest__card h1 {
  line-height: 49px;
  font-size: 36px;
  margin: 0;
}

<<<<<<< HEAD
=======
.invest__motivation {
}

>>>>>>> 4f8909487ba08ffdfca8871d00f4cc7309915937
.invest__motivation h3 {
  font-size: 18px;
  line-height: 25px;
}

.header {
  display: flex;
  flex-direction: column;
}

.header__title {
  display: flex;
  justify-content: space-between;
  font-size: 18px;
  line-height: 25px;
  color: #58506b;
  font-weight: 600;
}

.header__title--welcome {
  font-style: normal;
  font-weight: 600;
  font-size: 18px;
  line-height: 25px;
}
.icon {
  width: 50px;
  height: 50px;
}
</style>
