<template>
  <div>
    <h2>{{ card.name }}</h2>
    <h3>{{ card.price }}</h3>
    <slot></slot>
  </div>
</template>

<script setup>
defineProps({
  card: {
    type: Object,
    required: true,
  },
})
</script>

<style scoped>
div {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-around;
  height: 300px;
  width: 200px;
  border: 3px solid black;
}
</style>