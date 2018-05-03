<template>
  <div id="app">
  

    <h1 class="text-center mt-5 container">Titolo Ex DOM</h1>

 

     <div class="panel-contener bg-success mt-5 container p-4">
        <div id="exo-4-panel" class="panel text-center active">
            <div class="row text-center">
                <div id="div1" class=" col-5 bg-secondary ">
                    <div v-if="affiche" id="divrossa" class=" bg-danger my-5 mx-5">
                        <h2>Lorem </h2>
                    </div>
                </div>
                <div id="div2" class=" col-5 bg-secondary ml-5">
                    <div v-if="!affiche" id="divrossa" class=" bg-danger my-5 mx-5">
                        <h2>Lorem </h2>
                    </div>
                </div>
            </div>
            <button v-on:click="scambio" class="p-3 mt-5">Eccomi</button>
            <h2 id="score">Score</h2>
        </div>

    </div>


  </div>
</template>




<script>
export default {
  data() {
    return {
      affiche: true
    };
  },
  methods: {
    scambio: function() {
      this.affiche = !this.affiche;
    }
  }
};
</script>


<style lang="scss">

</style>
