<template>
  <div id="app">
  

    <h1 class="text-center mt-5 container">Titolo Ex DOM</h1>


     <div class="panel-contener bg-success mt-5 container p-4">
        <div id="exo-5-panel" class="panel text-center active">
           <h2>Generer des elements du DOM </h2>
    <p>Cliquer sur le bouton ci-dessous pour generer des oeufs </p>
    <button v-on:click= "aggiungi" class="add-egg btn btn-success">Ajputer un oeuf</button>
    <div class="row">
    <div :class="panier" v-for="(mucca,index) in panier" :key="index">
      <img class=" img1 " src="../assets/logo.png" alt="">
    </div>
    </div>
        </div>
                                      
    </div>


  </div>
</template>




<script>
export default {
  data() {
    return {
      panier: []
    };
  },
  methods: {
    aggiungi() {
      this.panier.push("hello");
    }
  }
};
</script>


<style lang="scss">

</style>
