<script setup>
import { RouterView, RouterLink } from "vue-router"
</script>

<template>
  <div>
    <RouterLink active-class="active" to="/">Home</RouterLink>
    <RouterLink active-class="active" to="/about">About</RouterLink>
    <RouterView />
  </div>
</template>

<style scoped>
  .active {
    font-weight: 900;
    color: rgb(153, 104, 14)
  }
</style>
