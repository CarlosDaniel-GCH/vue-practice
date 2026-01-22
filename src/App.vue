<script setup>
// Componentes
import defineProps from './components/defineProps.vue'
import vFor from './components/v-for.vue';
import VIf from './components/v-if.vue';
import VModel from './components/v-model.vue'
import Ref from './components/ref.vue';
import Click from './components/click.vue';
import vBind from './components/v-bind.vue';
</script>

<template>
  <!-- Descomenta el componente que quieras utilizar -->
  <!-- <defineProps msg="Esto es un mensaje" :user="{nombres : 'Pedro' , apellidos : 'Sanchez', edad: 43}" />
  <vFor />
  <VIf />
  <VModel />
  <Ref />
  <Click /> -->
  <vBind />
</template>

<style scoped>
</style>