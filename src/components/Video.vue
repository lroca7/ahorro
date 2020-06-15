<template>
  <section class="video">
    <div class="header">
      <div class="header__title">
        <p class="header__title--welcome">Las Pautas del ahorro</p>
        <div class="icon__container">
          <img
            class="icon"
            src="https://img.icons8.com/carbon-copy/100/000000/bell.png"
          />
        </div>
      </div>
    </div>
    <div class="videos">
      <img src="../assets/video.png" />
      <div class="video__description">
        <p class="title">Esto es AHORRO</p>
        <p class="description">
          Conoce como nuestro RoboAdvisor crea el mejor portafolio de inversión
          para ti
        </p>
      </div>
    </div>
    <div class="counter">
      <div class="counter_circle"></div>
      <div class="counter_circle"></div>
      <div class="counter_circle"></div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Video"
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
.counter {
  display: flex;
}
.counter_circle {
  position: static;
  width: 10px;
  height: 10px;
  left: 0px;
  top: 5px;

  background: linear-gradient(
      180deg,
      rgba(44, 82, 216, 0) 0%,
      rgba(44, 82, 216, 0.4) 100%
    ),
    #54d1ed;
  background-blend-mode: multiply, normal;

  /* Inside Auto Layout */

  flex: none;
  order: 0;
  align-self: center;
  margin: 10px 0px;
  margin-right: 5px;

  border-radius: 10px;
}

.description {
  font-style: normal;
  font-weight: normal;
  font-size: 12px;
  line-height: 16px;
  display: flex;
  align-items: center;
  letter-spacing: -0.03em;
}

.title {
  font-style: normal;
  font-weight: 600;
  font-size: 24px;
  line-height: 33px;
}
.video__description {
  background: linear-gradient(
      180deg,
      rgba(44, 82, 216, 0) 0%,
      rgba(44, 82, 216, 0.4) 100%
    ),
    #54d1ed;
  background-blend-mode: multiply, normal;
  padding: 30px;
  margin-top: -14%;
}

.video__description p {
  padding: 0;
  margin: 0;
  color: #ffffff;
}

.videos img {
  width: 100%;
  border-radius: 20px;
}

.videos {
  display: flex;
  flex-direction: column;
}
</style>
