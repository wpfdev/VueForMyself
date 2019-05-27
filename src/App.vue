<template>
  <div>
    <h1>Hello World</h1>
    <app-car></app-car>
  </div>
</template>

<script>
import Car from "./Components/Car.vue";

export default {
  data() {
    return {
      msg: "Welcome to Vue"
    };
  },
  components: {
    appCar: Car
  }
};
</script>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  padding: 30px;
  a {
    font-weight: bold;
    color: #2c3e50;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
