<template>
  <section class="menu">
    <ul class="menu__list">
      <li>
        <img src="../assets/home.png" />
        <a>Inicio</a>
      </li>
      <li>
        <img src="../assets/list.png" />
        <a>Historial</a>
      </li>
      <li>
        <div class="elipse"><img src="../assets/plus.png" /></div>
        <a class="elipse__a">Ahorrar</a>
      </li>
      <li>
        <img src="../assets/user.png" />
        <a>Mi perfil</a>
      </li>
      <li>
        <img src="../assets/more_options.png" />
        <a>Más</a>
      </li>
    </ul>
  </section>
</template>

<script>
export default {
  name: "Menu"
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.elipse__a {
  position: absolute;
  bottom: 70px;
}
.elipse {
  width: 50px;
  height: 50px;

  background: linear-gradient(
      180deg,
      rgba(44, 82, 216, 0) 0%,
      rgba(44, 82, 216, 0.4) 100%
    ),
    #54d1ed;
  background-blend-mode: multiply, normal;

  border-radius: 50px;
  position: absolute;
  bottom: 5%;

  display: flex;
  justify-content: center;
  align-items: center;
}
.menu__list a {
  font-style: normal;
  font-weight: normal;
  font-size: 10px;
  line-height: 14px;
  /* identical to box height */

  display: flex;
  align-items: center;
  text-align: center;
  letter-spacing: -0.03em;

  /* 25% */

  color: #a99dc6;
}
.menu__list li img {
  width: 20px;
  height: 20px;
}
.menu__list li {
  height: inherit;
  display: flex;
  align-items: center;
  padding: 0 10px;

  display: flex;
  flex-direction: column;
}
.menu__list ul {
  margin: 0;
  padding: 0;
  list-style: none;
}
.menu__list {
  display: flex;
  padding: 0;
  margin: 0;
  align-items: center;
  justify-content: space-between;

  width: 90%;
}
.menu {
  background: #ffffff;
  border-radius: 16px;
  height: 60px;
  display: flex;
  justify-content: center;
}
</style>
