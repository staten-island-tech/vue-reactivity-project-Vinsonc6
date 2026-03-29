<template>
  <div class="container">
    <CardComponent
      v-for="film in HorribleFilms"
      :key="film.name"
      :title="film.name"
      :year="film.yearReleased"
      :price="film.price"
      :image="film.image"
    />
  </div>
</template>

<script setup>
import { ref } from 'vue'
import CardComponent from "./components/CardComponent.vue"

const HorribleFilms = ref([
  {name: "Big Hero Six", yearReleased: 2014, price: 6.99, image: "/big hero 6.jpg"},
  {name: "Finding Dory", yearReleased: 2016, price: 6.99, image: "/Finding dory.jpg"},
  {name: "Cars 3", yearReleased: 2017, price: 5.99, image: "/Car 3.jpg"},
  {name: "Megamind vs. the Doom Syndicate", yearReleased: 2024, price: 8.00, image: "/megamind vs doom.jpg"},
  {name: "Star Wars: The Rise of Skywalker", yearReleased: 2019, price: 7.99, image: "/tom brady.jpg"},
  {name: "Mufasa: The Lion King", yearReleased: 2024, price: 5.99, image: "/Mustafa.jpeg"},
  {name: "The Good Dinosaur", yearReleased: 2015, price: 2.99, image: "/The good Dinosaur.jpg"},
  {name: "Shark Tale", yearReleased: 2004, price: 5.99, image: "/Shark Tale.webp"},
  {name: "The Hangover 3", yearReleased: 2013, price: 6.99, image: "/hangover 3.jpg"},
  {name: "Welcome to Derry", yearReleased: 2025, price: 10.99, image: "/WelcomeToDerry.jpg"},
  {name: "Daddy Doesn't Live Here Anymore", yearReleased: 2022, price: 3.99, image: "/tom brady.jpg"},
])
</script>

<style>
.container {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  padding: 20px;
}
</style>