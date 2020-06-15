<template>
  <section class="tips">
    <div class="tip" v-for="t in tips" :key="`${t.code}`">
      <div class="tip__text">
        <p class="tip__title">{{ t.title }}</p>
        <p class="tip__content">{{ t.content }}</p>
      </div>
      <div class="tip__img">
        <img src="../assets/tip.png" />
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Tip",

  data() {
    return {
      tips: [
        {
          code: 1,
          title: "10 gastos que debes evitar",
          content: `Aunque el 66% de los adultos recibió 
                    educacion para el ahorro, apenas el 44%
                    ahorra de manera formal.`
        },
        {
          code: 2,
          title: "10 gastos que debes evitar",
          content: `Aunque el 66% de los adultos recibió 
                    educacion para el ahorro, apenas el 44%
                    ahorra de manera formal.`
        },
        {
          code: 3,
          title: "10 gastos que debes evitar",
          content: `Aunque el 66% de los adultos recibió 
                    educacion para el ahorro, apenas el 44%
                    ahorra de manera formal.`
        }
      ]
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
.tip__img img {
  width: 68px;
  height: 68px;
  border-radius: 20px;
}
.tip__content {
  font-style: normal;
  font-weight: normal;
  font-size: 10px;
  line-height: 14px;
  letter-spacing: -0.03em;

  color: #58506b;
}
.tip__title {
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 21px;
  color: #817699;
}
.tip__text {
  display: flex;
  flex-direction: column;
  width: 70%;
}
.tip {
  margin-bottom: 1px;
  border-radius: 20px;
  display: flex;
  justify-content: space-between;
}
.tips {
  display: flex;
  flex-direction: column;
  padding: 20px;
}
</style>
