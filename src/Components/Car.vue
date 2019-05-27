<template>
  <div>
    <h3>{{ carName }}</h3>
    <p>Year: {{carYear}}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      carName: "Ford",
      carYear: 2019
    };
  }
};
</script>

<style lang="scss" scoped>
</style>