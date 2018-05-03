<template>
  <div id="app">


    <h1 class="text-center mt-5 container">Titolo Ex DOM VUE</h1>

    <div class="mt-5 text-center container" id="button">
        <button @click="" data-position="1" class="btn btn-dark px-3 mx-3 ">Ex.1</button>
        <button @click="" data-position="2" class="btn btn-dark px-3 mx-3">Ex.2</button>
        <button @click="" data-position="3" class="btn btn-dark px-3 mx-3 ">Ex.3</button>
        <button @click="" data-position="4" class="btn btn-dark px-3 mx-3">Ex.4</button>
        <button @click="" data-position="5" class="btn btn-dark px-3 mx-3">Ex.5</button>
        <button @click="" data-position="6" class="btn btn-dark px-3 mx-3">Ex.6</button>
        <button @click="" data-position="7" class="btn btn-dark px-3 mx-3">Ex.7</button>
        <button @click="" data-position="8" class="btn btn-dark px-3 mx-3">Ex.8</button>
        <button @click="" data-position="9" class="btn btn-dark px-3 mx-3">Ex.9</button>
        <button @click="" data-position="10" class="btn btn-dark px-3 mx-3">Ex.10</button>
    </div>

    <div class="panel-contener bg-secondary mt-5 container p-4">
      <ex1></ex1>
      <ex2></ex2>
      <ex3></ex3>
      <ex4></ex4>
      <ex5></ex5>
      <ex6></ex6>
      <ex7></ex7>
    </div>

  </div>


 
</template>




<script>
import ex1 from "./components/ex1.vue";
import ex2 from "./components/ex2.vue";
import ex3 from "./components/ex3.vue";
import ex4 from "./components/ex4.vue";
import ex5 from "./components/ex5.vue";
import ex6 from "./components/ex6.vue";
import ex7 from "./components/ex7.vue";

export default {
  name: "app",
  components: {
    ex1,
    ex2,
    ex3,
    ex4,
    ex5,
    ex6,
    ex7
  }
};
</script>


<style lang="scss">
@import "../node_modules/bootstrap/scss/bootstrap.scss";
@import "../node_modules/font-awesome/css/font-awesome.min.css";
</style>
