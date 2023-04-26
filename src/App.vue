<script setup>
import { RouterView, RouterLink } from "vue-router"
</script>

<template>
  <div>
    <RouterLink to="/">Home</RouterLink>
    <RouterLink to="/about">About</RouterLink>
    <RouterView />
  </div>
</template>

<style scoped>

</style>
