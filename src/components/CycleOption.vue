<template>
    <div>Hola mundo</div>
</template>

<script setup lang="ts">
import { onMounted, onUpdated } from "vue";

onMounted(() => {
    console.log("Mounted");
});

onUpdated(() => {
    console.log("Updated");
});
</script>

<style scoped></style>