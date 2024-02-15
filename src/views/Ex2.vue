<template>
  <div>
    <div class="title"><h1>Les observateurs</h1></div>
    <div class="ex">
      <h1>Passez moi en rouge</h1> <!-- ajoutez la liaison de la classe dynamique ici -->
    </div>
  </div>
</template>

<script setup>
import {ref} from 'vue'

const titleClass = ref('title');

</script>

<style>
.title {

}
</style>
