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
      <div class="goal">
        <img src="../assets/palmera.png" />
        <p>Viaje a islas canarias</p>
        <pie-chart
          :donut="true"
          :colors="['#FAF9FD', '#54D1ED']"
          :data="[
            ['$8.000.000', 80],
            ['$1.630.000', 20]
          ]"
        ></pie-chart>
      </div>
      <div class="goal">
        <img src="../assets/computer.png" />
        <p>Macbook Pro</p>

        <pie-chart
          :donut="true"
          :colors="['#54D1ED', '#FAF9FD']"
          :data="[
            ['$0', 0],
            ['$7.000.000', 100]
          ]"
        ></pie-chart>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Goal",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
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
  width: 150px;
}

.goal:first-child {
  margin-left: 3%;
}
</style>
