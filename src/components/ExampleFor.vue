<template>
    <ul>
        <li v-for="country in countries" :key="country.code">{{ country.name }}</li>
    </ul>
</template>

<script setup lang="ts">
import { Ref, ref } from 'vue'
interface ICountry {
    code: string,
    name: string
}
let countries: Ref<Array<ICountry>> = ref([
    {
        code: 'es',
        name: 'Spain'
    },
    {
        code: 'fr',
        name: 'France'
    },
    {
        code: 'en',
        name: 'UK'
    },
    {
        code: 'it',
        name: 'Italy'
    },
    {
        code: 'pt',
        name: 'Portugal'
    },
    {
        code: 'de',
        name: 'Germany'
    }
])
</script>

<style scoped></style>