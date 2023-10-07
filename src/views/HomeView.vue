<script setup>
import TheWelcome from '../components/TheWelcome.vue'
import { api } from '../axios.js'

api.get('http://api.harundemir.kim/WeatherForecast').then((response) => {
  console.log(response)
})

api.get('https://localhost:7045/WeatherForecast').then((response) => {
  console.log(response)
})
</script>

<template>
  <main>
    <TheWelcome />
  </main>
</template>
