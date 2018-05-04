<template >

  <li  class=" mt-4  bg-white icon d-flex justify-content-between" :class="{'done':barrato}">
    <div class="nome ajouter ml-4"> <p :class="{'barrato':barrato}" class="my-4">{{name}}</p></div>
    <form v-if="form" action="" class="form-inline justify-content-center " id="form-task">
        <input v-model="name" type="text" id="input-task" class="form-control" placeholder="new task">
        <button @click="ok" type="submit" class="btn btn-primary" id="btn-add-task">ok</button>
    </form>
    <div id="divicone" class="my-4">
      <i @click="verifie" class="vero mr-3 fa fa-check" aria-hidden="true"></i>
      <i @click="canc" class=" mr-3 fa fa-times-circle-o" aria-hidden="true"></i>
      <i @click="modify" class="modifica fa fa-pencil" aria-hidden="true"></i>
    </div> 
  </li>

</template>

<script lang="js">


  export default  {
    name: 'ex-7-comp',
    components : {
      
    },
    props: ["texte"],
    mounted() {

    },
    data() {
      return {
        
        barrato : false,
        form : false,
        name: this.texte,
 
       
      }
    },
    methods: {
      verifie() {
      this.barrato = !this.barrato

    },
      canc() {
        this.$emit("canc",this.name)
    },
    modify() {
        this.form = !this.form 
      },
      ok(){
        this.form = false
      },
    },
    computed: {
      
    }
}
</script>



<style scoped lang="scss">
.barrato {
  text-decoration: line-through;
}
</style>
