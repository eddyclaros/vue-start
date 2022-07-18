<template>
  <h1>Our first Component</h1>
  
  
  <CarOptions></CarOptions>
  <hr>
  <CarComposition></CarComposition>
</template>

<script>
import CarOptions from "./components/CarOptions.vue";
import CarComposition from "./components/CarComposition.vue";

export default {
  components:{
    CarOptions,
    CarComposition
}
}
</script>

<style>

</style>