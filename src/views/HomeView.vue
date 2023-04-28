<template>
  <div>
    <h1>Home View</h1>
    <div class="cars">
      <RouterLink :to="`/cars/${car.id}`" v-for="car in cars" :key="car.id">{{ car.name }}</RouterLink>
    </div>
  </div>
</template>

<script setup>
import { RouterLink } from "vue-router"
import cars from "../data/cars.json"
</script>


<style>
.cars {
  display: flex;
  background: white;
}

.cars a {
  text-decoration: none;
  color: black;
  width: 100%;
  box-shadow: 1px 1px 10px rgba(50, 0, 0, 0.388);
  margin: 10px;
}
</style>
