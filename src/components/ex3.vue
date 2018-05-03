<template>
  <div id="app">
  

    <h1 class="text-center mt-5 container">Titolo Ex DOM</h1>


    <div class="panel-contener bg-secondary mt-5 container p-4">
        <div id="exo-3-panel" class="panel active">
            <h2>welcome
                <span>{{scritta}}</span>
            </h2>
            <p>écriver dans l'input ci-dessous le nom de la personne qui vous voulez accueillir
                <br> lorsque vous cliquez sur le bouton "go" le nom que vous avez ajouter dans l'input sera alors mis dans le
                span du h2 et l'inp ut sera alors vidé de toute contenu. Attention, interdiction de toucher à l'html</p>
            <form action="">
                <input v-model="inp" type="text">
                <button @click.prevent="affiche">go</button>
            </form>
        </div>

    </div>


  </div>
</template>




<script>
export default {
  name: "ex3",
  data() {
    return {
      scritta: "inconnu",
      inp: ""
    };
  },
  methods: {
    affiche: function() {
      this.scritta = this.inp;
      this.inp = "";
    }
  }
};
</script>


<style lang="scss">

</style>
