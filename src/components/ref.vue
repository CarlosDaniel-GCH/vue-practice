<script setup>
import { ref, onMounted } from 'vue'

const usuarios = ref([])

const lista = ["user1", "user2", "user3", "user4"]

onMounted(() => {
    usuarios.value.push(lista)
})

</script>

<template>
    <div v-for="user in usuarios">
        {{ user }}
    </div>
</template>