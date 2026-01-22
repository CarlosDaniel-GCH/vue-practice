<script setup>
defineProps({
  msg: String,
  user: {
    nombres: String,
    apellidos: String,
    edad: Number
  }
})
</script>

<template>
  <div>
    <span>{{ msg }}</span>
    <h1>{{ user.nombres }}</h1>
    <h2>{{ user.apellidos }}</h2>
    <h3>{{ user.edad }} años</h3>
  </div>
</template>

<style scoped>
</style>