<script setup>
  // Componentes
  import defineProps from './components/defineProps.vue'
  import vFor from './components/v-for.vue';
  import VIf from './components/v-if.vue';
</script>

<template>
  <!-- Plantilla para visualizar cada componente -->
  <defineProps msg="Esto es un mensaje" :user="{nombres : 'Pedro' , apellidos : 'Sanchez', edad: 43}" />
  <vFor />
  <VIf />
</template>

<style scoped>
</style>