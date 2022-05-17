<template>
  <div class="container">
    <img src="./assets/logo.svg" alt="logo vue" width="200" height="200" />
    <small><h1>Hola mundo desde VUE.JS 3</h1> </small>
    <hr />
    <h2>Contador {{ contador }}</h2>
    <button @click="sumar">+1</button>
    <button @click="restar">-1</button>
    <button @click="reset">reset</button>
  </div>
  <div>
    <img
      class="vite"
      src="./assets/logo_vite.svg"
      alt="logo vite"
      width="200"
      height="200"
    />
  </div>
</template>

<script>
export default {
  data: () => ({
    contador: 20,
  }),
  methods: {
    sumar() {
      this.contador++;
    },
    restar() {
      this.contador--;
    },
    reset() {
      this.contador = 0;
    },
  },
};
</script>

<style scoped>
/* @import "./assets/base.css"; */

.container {
  text-align: center;
}

small {
  color: #666;
}

h1 {
  font-weight: bolder;
  color: #666;
}

h2 {
  font-size: 2rem;
}

button {
  cursor: pointer;
  font-size: 1.5rem;
  margin: 0px 6px;
}

.vite {
  display: flex;
  margin: 30px auto;
}
</style>
