<script setup>
    const lista = [1,2,3,4,5,6,7,8,9,10]

</script>

<template>
    <div v-if="lista.length >= 9">
        <h3>Mi Lista de Números:</h3>

        <ul>
            <li v-for="item in lista" :key="item">
                Número: {{ item }}
            </li>
        </ul>
    </div>
</template>