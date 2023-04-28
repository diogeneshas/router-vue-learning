<template>
  <div>
    <h1>Car View</h1>
    <p>{{car.name}}</p>
    <p>{{car.year}}</p>
    <p>{{car.price}}</p>
    <button @click="router.push(`/cars/${carId}/contact`)">Click for contact</button>
    <RouterView />
  </div>
</template>

<script setup>
import { useRoute, RouterView, useRouter } from "vue-router"
import cars from "../data/cars.json"

const route = useRoute()
const router = useRouter()
const car = cars.find(c => c.id === parseInt(route.params.id))
const carId = parseInt(route.params.id)

</script>
