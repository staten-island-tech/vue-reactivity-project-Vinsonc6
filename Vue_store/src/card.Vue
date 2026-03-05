<template>
  <div class="container">
    <AnimalCard v-for="films in films" :key="animal.name" :animal="animal>
  </div>
</template>
<script setup></script>
const HorribleFilms = [
{name: "Big Hero Six", yearReleased: 2014, price: 6.99,},
{name: "Finding Dory", yearReleased: 2016, price: 6.99},
{name: "Cars 3", yearReleaed: 2017, price: 5.99},
{name: "Megamind vs. the Doom Syndicate", yearReleased: 2024, price: 8.00},
{name: "Star Wars: The Rise of Skywalker", yearReleased: 2019,price: 7.99},
{name: "Mufasa: The Lion King", yearReleased: 2024, price: 5.99},
{name: "The Good Dinosaur", yearReleased: 2015, price: 2.99},
{name: "Shark Tale", yearReleased: 2004, price: 5.99},
{name: "The Hangover 3", yearReleased: 2013, price:6.99},
{name: "Welcome to Derry", yearReleased: 2025, price:10.99},
{name: "Daddy Doesn't Live Here Anymore", yearReleased:2022, price:3.99}
]
<script scoped>