<template>
  <div>
    <div class="title"><h1>Le rendu conditionnel</h1></div>
    <div class="ex">
      <button @click="">ON/OFF</button>
      <h1 class="jour">☀️Jour</h1>
      <h1 class="nuit">🌙Nuit</h1>
    </div>
  </div>
</template>

<script setup>
import {ref} from "vue";
</script>

<style scoped>
.jour {
  background-color: #f2f2f2;
  color: crimson;
  padding: 10px;
  margin: 10px;
}

.nuit {
  background-color: #181818;
  color: darkcyan;
  padding: 10px;
  margin: 10px;
}
</style>