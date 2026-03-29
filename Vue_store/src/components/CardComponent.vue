<template>
  <div class="card">
    <img :src="image" :alt="title" />
    <div class="card-body">
      <h3>{{ title }}</h3>
      <p>{{ year }}</p>
      <p>${{ price.toFixed(2) }}</p>
    </div>
  </div>
</template>

<script setup>
defineProps({
  title: String,
  year: Number,
  price: Number,
  image: String
})
</script>

<style scoped>
.card {
  border: 1px solid #ccc;
  border-radius: 8px;
  overflow: hidden;
  width: 300px;
}
.card img {
  width: 100%;
}
.card-body {
  padding: 12px;
}
</style>