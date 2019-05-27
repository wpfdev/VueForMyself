<template>
  <div class="car">
    <h3>Model: {{ carName }}</h3>
    <p>Year: {{carYear}}</p>
  </div>
</template>

<script>
export default {
  props: ["carName", "carYear"]
};
</script>

<style lang="scss" scoped>
.car {
  border: 1px solid black;
  border-radius: 5px;
  padding: 10px;
  margin-bottom: 10px;
}
</style>