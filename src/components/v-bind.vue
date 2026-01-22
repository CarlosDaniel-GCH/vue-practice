<script setup>
import { reactive } from 'vue'

const usuario = reactive({
    id: 101,
    nombre: "Alex",
    apellido: "Rivera",
    estaActivo: true
})

</script>

<template>
    <!-- Tambien se puede usar " : " para abreviar en vez de v-bind -->
    <div>
        <span v-bind:key="usuario.id">
            {{ usuario.id }}
        </span>
        <h1>{{ usuario.nombre }} {{ usuario.apellido }}</h1>
        <span>
            Activo: {{ usuario.estaActivo }}
        </span>
    </div>
</template>