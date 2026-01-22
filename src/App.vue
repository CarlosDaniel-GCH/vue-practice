<script setup>
import defineProps from './components/defineProps.vue'
</script>

<template>
  <defineProps msg="Esto es un mensaje" :user="{nombres : 'Pedro' , apellidos : 'Sanchez', edad: 43}" />
</template>

<style scoped>
</style>