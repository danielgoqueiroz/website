<template>
  <div class="container">
    <header><Menu /></header>
    <NuxtLink to="/home">Home</NuxtLink>
    <NuxtLink to="/sobre">Sobre</NuxtLink>
    <NuxtLink to="/contato">Contato</NuxtLink>
    <Nuxt />
    <footer>Footer</footer>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>

<style>
body {
  font-family: 'montserrat', sans-serif;
}

.container {
  margin: 0;
  padding: 0;
  min-height: 100vh;
  box-sizing: border-box;
}

header {
  width: 100vw;
  background-color: #222;
  padding: 15px;
}
</style>
