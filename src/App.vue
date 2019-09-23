<template>
  <div id="app">
    <h1>Conversor de Moedas</h1>
    <div class="linha">
      <conversor moedaA="USD" moedaB="BRL" />
      <conversor moedaA="BRL" moedaB="USD" />
    </div>
    <div class="linha">
      <conversor moedaA="CAD" moedaB="BRL" />
      <conversor moedaA="BRL" moedaB="CAD" />
    </div>
    <div class="linha">
      <conversor moedaA="EUR" moedaB="BRL" />
      <conversor moedaA="BRL" moedaB="EUR" />
    </div>
  </div>
</template>

<script>
import Conversor from "./components/Conversor.vue";
export default {
  name: "app",
  components: {
    Conversor
  }
};
</script>

<style>
#app {
  margin: auto;
  max-width: 900px;
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.linha {
  margin-top: 40px;
  display: flex;
  justify-content: space-around;
}
</style>
