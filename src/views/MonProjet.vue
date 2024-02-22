<template>
  <div>
    <div v-if="weatherStore.weather">
      <p>Location: {{ weatherStore.weather.location.name }}</p>
      <p>Region: {{ weatherStore.weather.location.region }}</p>
      <p>Pays: {{ weatherStore.weather.location.country }}</p>
    </div>
    <div v-else>
      Loading weather information...
    </div>
  </div>
</template>

<script setup>

import {useWeatherStore} from "@/stores/weatherStore.js";

const weatherStore = useWeatherStore();

weatherStore.getCurrentWeather();

console.log(weatherStore.weather);


</script>
