<template>
  <div id="app">

    <div class="container mt-5">

      <FormTask v-model="newTask" @add="add" />

      <div class="row mt-3">

        <KanbanColumn titulo="Pendente" :tasks="arrPendencia" alert-class="alert-secondary" />
        <KanbanColumn titulo="Em Progresso" :tasks="arrProgredindo" alert-class="alert-primary" />
        <KanbanColumn titulo="Testar" :tasks="arrTeste" alert-class="alert-warning" />
        <KanbanColumn titulo="Feito" :tasks="arrFeito" alert-class="alert-success" />

      </div>

    </div>

  </div>
</template>

<script>
import KanbanColumn from './components/KanbanColumn.vue';
import FormTask from './components/FormTask.vue'
export default {
  name: 'App',
  components: { KanbanColumn, FormTask },
  data() {
    return {
      newTask: '',
      arrPendencia: [],
      arrProgredindo: [],
      arrTeste: [],
      arrFeito: [],
    };
  },
  methods: {
    add() {
      if (this.newTask) {
        this.arrPendencia.push({ name: this.newTask });
        this.newTask = "";
      }
    }
  }
}
</script>
