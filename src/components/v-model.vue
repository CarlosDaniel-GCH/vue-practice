<script setup>
    import { reactive } from 'vue'

    const formulario = reactive({
        nombre: '',
        apellidos: '',
        aceptarTerminos: false
    })

    const enviarFormulario = () => {
        console.log("Datos enviado: ", formulario)
    }
</script>

<template>
    <form @submit.prevent="enviarFormulario">
        <input type="text" v-model="formulario.nombre" placeholder="Nombres">

        <input type="text" v-model="formulario.apellidos" placeholder="Apellidos">

        <label>
            <input type="checkbox" v-model="formulario.aceptarTerminos">
            Acepto los terminos
        </label>

        <button type="submit">Enviar</button>
    </form>

    <pre>{{ formulario }}</pre>
</template>