<template>
    <form>
        <input type="text" v-model="inputText">
    </form>
    <h3>{{ inputText }}</h3>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
export default defineComponent({
    data() {
        return { inputText: '' }
    }
});
</script>

<style scoped></style>