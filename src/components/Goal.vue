<template>
  <section class="goals">
    <div class="header">
      <div class="header__title">
        <p class="header__title--welcome">Tus metas</p>
        <div class="icon__container">
          <img
            class="icon"
            src="https://img.icons8.com/carbon-copy/100/000000/bell.png"
          />
        </div>
      </div>
    </div>
    <div class="goals__container">
      <div class="goal" v-for="g in goals" :key="`${g.name}`">
        <img src="../assets/palmera.png" /> 
        <p>{{ g.name }}</p>
        <vc-donut
          background="white"
          foreground="white"
          :size="50"
          unit="px"
          :thickness="30"
          has-legend
          legend-placement="right"
          :sections="g.sections"
          :total="100"
          :start-angle="0"
          :auto-adjust-text-size="true"
        >
          <h1>20%</h1>
        </vc-donut>
      </div>
      <!-- <div class="goal">
        <img src="../assets/computer.png" />
        <p>{{goals[1].name}}</p>
        <vc-donut
          background="white"
          foreground="white"
          :size="50"
          unit="px"
          :thickness="30"
          has-legend
          legend-placement="right"
          :sections="goals[0].sections"
          :total="100"
          :start-angle="0"
          :auto-adjust-text-size="true"
        >
          <h1>0%</h1>
        </vc-donut>
      </div> -->
    </div>
  </section>
</template>

<script>
export default {
  name: "Goal",
  props: {
    msg: String
  },
  data() {
    return {
      goals: [
        {
          name: "Viaje a Islas Canarias",
          img: "../assets/palmera.png",
          sections: [
            { label: "$1.630.000", value: 20, color: "#51CAEC" },
            { label: "$8.000.000", value: 80, color: "#FAF9FD" }
          ]
        },
        {
          name: "Macbook Pro",
          img: "../assets/computer.png",
          sections: [
            { label: "$0", value: 0, color: "#51CAEC" },
            { label: "$7.000.000", value: 100, color: "#FAF9FD" }
          ]
        }
      ]
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
.cdc-legend-item span:last-child {
  font-style: normal;
  font-weight: 600;
  font-size: 12px;
  line-height: 16px;
  letter-spacing: -0.03em;
}
.cdc-legend-item-color {
  display: none;
}
.goals__container {
  display: flex;
  justify-content: space-between;
  color: #58506b;
}

.goal img {
  width: 40px;
  height: 40px;
}

.goal {
  /* White */

  background: #ffffff;
  /* Card shadow soft */

  box-shadow: 0px 8px 20px rgba(197, 166, 236, 0.05);
  border-radius: 20px;
  padding: 20px;
  width: 158px;
}

.goal > p {
  font-weight: 600;
  font-size: 14px;
  line-height: 21px;
  /* or 150% */

  display: flex;
  align-items: center;
  letter-spacing: -0.01em;

  /* 50% */

  color: #817699;
  width: 118px;
  height: 42px;
}

.goal:first-child {
  margin-right: 3%;
}
</style>
