<template>
  <div id="app">
      


    <div id="exo-7-panel" class="panel active">
            <h2 class="text-center">Todo list</h2>
            <form action="" class="form-inline justify-content-center " id="form-task">
                <input v-model="value" type="text" id="input-task" class="form-control" placeholder="new task">
                <button @click="ajouter" type="submit" class="btn btn-primary" id="btn-add-task">Add task</button>
            </form>
            <h2 class="mt-5">
                <small>Filtre :</small>
                <button class="btn btn-success filtre" id="all" @click="filtrere">All</button>
                <button class="btn btn-success filtre" id="todo" @click="filtrere">Todo</button>
                <button class="btn btn-success filtre" id="done" @click="filtrere">Done</button>
            </h2>
            <ul class="list-group flex-column" :class="newfilter" id="list-tasks">
                <ex7comp v-for="(mucca,index) in contenitore" :key="index" :texte="mucca" > </ex7comp>
            </ul>
        </div>


  </div>
</template>




<script>
import ex7comp from "./ex7comp.vue";

export default {
  components: {
    ex7comp
  },
  data() {
    return {
      value: "",
      contenitore: [],
      newfilter: "all"
    };
  },
  methods: {
    ajouter() {
      this.contenitore.push(this.value);
      this.value = "";
    },
    filtrere(event) {
      this.newfilter = event.currentTarget.id;
      console.log(event.currentTarget.id);
    }
  }
};
</script>


<style lang="scss">
ul {
  &.todo {
    li.done {
      display: none !important;
    }
  }
  &.done {
    li.done {
      display: block !important;
    }
    li {
      display: none !important;
    }
  }
}
</style>
