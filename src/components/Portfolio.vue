<template>
  <section class="portfolio">
    <div class="header">
      <div class="header__title">
        <p class="header__title--welcome">Conoce tu portafolio</p>
        <div class="status">
          <span class="status__text">Estratega</span>
        </div>
      </div>
    </div>
    <div class="portafolio__resume">
      <div class="portafolio__resume--roboadvisor">
        <vc-donut
          background="white"
          foreground="white"
          :size="120"
          unit="px"
          :thickness="20"
          :sections="sections"
          :total="100"
          :start-angle="0"
          :auto-adjust-text-size="true"
        > 
          <img class="portafolio__resume--img" src="../assets/robot.png" />
          <p class="text__robot">RoboAdvisor</p>
          <p class="text__fondos">10 Fondos</p>
        </vc-donut>

        <div class="portafolio__product">
          <div class="portafolio__product--header">
            <img
              class="portafolio__product--logo"
              src="../assets/skandia.png"
            />
            <div class="percent">
              <span class="percent__text">15%</span>
            </div>
          </div>

          <p class="portafolio__product--activo">FIC Old Mutual Efectivo</p>
          <p class="portafolio__product--account">$240.000</p>
          <p class="portafolio__product--type">Tipo de activo</p>
          <p class="portafolio__product--rent">Renta fija</p>
          <p class="portafolio__product--deposit">Depósito a la fija</p>
        </div>
      </div>
      <p class="portafolio__product--note">
        Tu dinero se invierte de la forma más efeciente de acuerdo al perfil de
        riesgo asignado por nuestro RoboAdvisor
      </p>
    </div>
  </section>
</template>

<script>
export default {
  name: "Portfolio",
  props: {
    msg: String
  },

  data() {
    return {
      sections: [
        { value: 10, color: "#41CF69" },
        { value: 10, color: "#C3C0CA" },
        { value: 10, color: "#C9C7D0" },
        { value: 10, color: "#D1CED6" },
        { value: 10, color: "#D7D5DB" },
        { value: 10, color: "#DEDCE1" },
        { value: 10, color: "#E4E3E7" },
        { value: 10, color: "#EBEAED" },
        { value: 10, color: "#F2F1F3" },
        { value: 10, color: "#F9F8F9" }
      ]
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.portafolio__product--note {
  font-weight: normal;
  font-size: 10px;
  line-height: 14px;
  display: flex;
  align-items: center;
  letter-spacing: -0.03em;

  /* 75% */

  color: #58506b;
}

.portafolio__product--header {
  display: flex;
}

.percent__text {
  font-weight: 600;
  font-size: 10px;
  line-height: 14px;
  /* identical to box height */

  text-align: right;
  letter-spacing: -0.03em;

  /* White */

  color: #ffffff;

  /* Inside Auto Layout */

  flex: none;
  order: 0;
  align-self: center;
  margin: 10px 0px;
}

.percent {
  display: flex;
  /* flex-direction: row; */
  padding: 1px 8px;
  /* position: absolute; */
  width: 36px;
  height: 15px;
  /* left: 111px; */
  /* top: 0px; */
  background: #41cf69;
  border-radius: 6px;

  margin-left: 10%;
}

.portafolio__product p {
  padding: 5px 0;
}
.portafolio__product--deposit {
  font-weight: normal;
  font-size: 10px;
  line-height: 14px;
  letter-spacing: -0.03em;

  /* 75% */

  color: #58506b;
}

.portafolio__product--rent {
  font-weight: normal;
  font-size: 10px;
  line-height: 14px;
  letter-spacing: -0.03em;

  /* 75% */

  color: #58506b;
}
.portafolio__product--type {
  font-weight: 600;
  font-size: 10px;
  line-height: 14px;
  /* identical to box height */

  display: flex;
  align-items: center;
  letter-spacing: -0.03em;

  /* Success */

  color: #41cf69;
}

.portafolio__product--account {
  font-weight: 600;
  font-size: 12px;
  line-height: 16px;
  display: flex;
  align-items: center;
  letter-spacing: -0.03em;
  color: #58506b;
}

.portafolio__product--activo {
  font-weight: normal;
  font-size: 12px;
  line-height: 16px;
  display: flex;
  align-items: center;
  letter-spacing: -0.03em;

  /* 75% */

  color: #58506b;

  height: 16px;
}

.portafolio__product--logo {
  width: 90px;
}

.text__fondos {
  font-weight: normal;
  font-size: 12px;
  line-height: 16px;
  display: flex;
  align-items: center;
  text-align: center;
  letter-spacing: -0.03em;

  /* 75% */

  color: #58506b;
}

.text__robot {
  font-weight: normal;
  font-size: 10px;
  line-height: 14px;
  /* identical to box height */

  display: flex;
  align-items: center;
  text-align: center;
  letter-spacing: -0.03em;

  /* 50% */

  color: #817699;
}

.portafolio__resume--roboadvisor {
  display: flex;
  justify-content: space-between;
  margin-bottom: 20%;
}

.portafolio__resume {
  display: flex;
  flex-direction: column;

  background: #ffffff;
  /* Card shadow soft */

  box-shadow: 0px 8px 20px rgba(197, 166, 236, 0.05);
  border-radius: 20px;

  padding: 20px;
}

.portafolio__resume p {
  margin: 0;
}

.portafolio__resume--img {
  width: 40px;
  height: 40px;
}

.status {
  background: #e4ffee;
  /* Success */

  border: 0.5px solid #41cf69;
  box-sizing: border-box;
  border-radius: 10px;

  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;

  padding: 3px 10px;

  /* position: absolute; */
  width: 64px;
  height: 21px;
  /* right: 24px;
    top: 800px; */

  margin-right: 24px;
}

.status__text {
  color: #41cf69;
  font-family: Open Sans;
  font-style: normal;
  font-weight: 600;
  font-size: 10px;
  line-height: 14px;
  display: flex;
  align-items: center;
  text-align: center;
  letter-spacing: -0.03em;
}

.header__title {
  align-items: baseline;
}
</style>
