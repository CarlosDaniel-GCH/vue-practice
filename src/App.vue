<script setup>
  // Componentes
  import defineProps from './components/defineProps.vue'
  import vFor from './components/v-for.vue';
</script>

<template>
  <!-- Plantilla para visualizar cada componente -->
  <defineProps msg="Esto es un mensaje" :user="{nombres : 'Pedro' , apellidos : 'Sanchez', edad: 43}" />
  <vFor />
  
</template>

<style scoped>
</style>