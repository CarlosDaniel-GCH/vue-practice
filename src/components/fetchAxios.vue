<script setup>
import { ref, onMounted } from 'vue'

const pokemons = ref([])

const getPokemons = async () => {
    try{
        const API_URL = "https://pokeapi.co/api/v2/pokemon"
        const response = await fetch(API_URL)
        if(!response.ok) throw new Error("Error en la peticion")
        const data = await response.json()
        pokemons.value = data.results
    }
    catch(e){
        console.log("Error: ", e)
    }
}

onMounted(() => {
    getPokemons()
})
</script>

<template>
    <div v-for="pokemon in pokemons">
        {{ pokemon.name }}
    </div>
</template>