<template>
  <div>
    <h1>{{ title }}</h1>
    <app-car carName="Ford" :carYear="2019"></app-car>
    <app-car :carName="carNameFromParent" :carYear="2018"></app-car>
  </div>
</template>

<script>
import Car from "./Components/Car.vue";

export default {
  data() {
    return {
      title: "Car Sale",
      carNameFromParent: "BMW" //свойство можно передать в параметр компонента
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
