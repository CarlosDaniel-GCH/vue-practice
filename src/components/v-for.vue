<script setup>
    const lista = ["Primer Elemento", "Segundo Elemento", "Tercer Elemento", "Cuarto Elemento", "Quinto Elementos"]
</script>

<template>
    <div v-for="item in lista">
        {{ item }}
    </div>
</template>