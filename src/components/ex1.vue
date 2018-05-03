<template>
  <div id="app">
  

    <h1 class="text-center mt-5 container">Titolo Ex DOM</h1>



    <div class="panel-contener bg-secondary mt-5 container p-4">
        <div id="exo-1-panel" class="panel active">
            <h2>{{message}}</h2>
            <p>cambiare il contenuto di h2 </p>
        </div>

    </div>


  </div>
</template>




<script>
export default {
  name: "ex1",
  data() {
    return {
      message: "Hello Vue !"
    };
  }
};
</script>


<style lang="scss">

</style>
