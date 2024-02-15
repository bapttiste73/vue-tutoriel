<template>
  <div>
    <div class="title"><h1>Les boucles</h1></div>
    <div class="ex">
      <form @submit.prevent="addTodo">
        <input v-model="newTodo">
        <button>Ajouter une tâche</button>
      </form>
      <ul>
        <li>
          {{ todos[0].text }}
          <button @click="removeTodo(todos[0])">X</button>
        </li>
        <li>
          {{ todos[1].text }}
          <button @click="removeTodo(todos[0])">X</button>
        </li>
        <li>
          {{ todos[2].text }}
          <button @click="removeTodo(todos[0])">X</button>
        </li>
      </ul>
    </div>
  </div>
</template>

<script setup>
import {ref} from "vue";
let id = 0

const newTodo = ref('')
const todos = ref([
  { id: id++, text: 'Apprendre le HTML' },
  { id: id++, text: 'Apprendre le JavaScript' },
  { id: id++, text: 'Apprendre Vue' }
])

function addTodo() {
  // ...
  newTodo.value = ''
}

function removeTodo(todo) {
}
</script>

<style scoped>
.jour{
  background-color: #f2f2f2;
  color: crimson;
  padding: 10px;
  margin: 10px;
}

.nuit{
  background-color: #181818;
  color: darkcyan;
  padding: 10px;
  margin: 10px;
}
</style>