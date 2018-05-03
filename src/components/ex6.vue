<template lang="html">

  <!-- Exercice 6 -->
            <div id="exo-6-panel" class="panel">
                <h2>Création calculatrice</h2>
                <h3>Niveau 1</h3>
                <input type="text" class="nb1"> +
                <input type="text" class="nb2">
                <button class="calc1">=</button>
                <span class="result1"></span>
                <h3>Niveau 2</h3>
                <table class="table table-dark">
                    <tr>
                        <td colspan="4">
                            <div class="resultat text-right"></div>
                            <input type="text" class="nbr text-right">
                        </td>
                    </tr>
                    <tr>
                        <td>
                            <button class="btn btn-default chiffre">1</button>
                        </td>
                        <td>
                            <button class="btn btn-default chiffre">2</button>
                        </td>
                        <td>
                            <button class="btn btn-default chiffre">3</button>
                        </td>
                        <td>
                            <button class="btn btn-primary operation">+</button>
                        </td>
                    </tr>
                    <tr>
                        <td>
                            <button class="btn btn-default chiffre">4</button>
                        </td>
                        <td>
                            <button class="btn btn-default chiffre">5</button>
                        </td>
                        <td>
                            <button class="btn btn-default chiffre">6</button>
                        </td>
                        <td>
                            <button class="btn btn-primary operation">-</button>
                        </td>
                    </tr>
                    <tr>
                        <td>
                            <button class="btn btn-default chiffre">7</button>
                        </td>
                        <td>
                            <button class="btn btn-default chiffre">8</button>
                        </td>
                        <td>
                            <button class="btn btn-default chiffre">9</button>
                        </td>
                        <td>
                            <button class="btn btn-primary operation">*</button>
                        </td>
                    </tr>
                    <tr>
                        <td>
                            <button class="btn btn-danger clear">C</button>
                        </td>
                        <td>
                            <button class="btn btn-default chiffre">0</button>
                        </td>
                        <td>
                            <button class="btn btn-success egal">=</button>
                        </td>
                        <td>
                            <button class="btn btn-primary operation">/</button>
                        </td>
                    </tr>
                </table>
            </div>

</template>

<script lang="js">
  export default  {
    name: 'ex-6',
    props: [],
    mounted() {

    },
    data() {
      return {

      }
    },
    methods: {

    },
    computed: {

    }
}
</script>

<style scoped lang="sass">

#exo-6-panel
  table.table
    width: 240px
    .resultat
        height: 24px

</style>
