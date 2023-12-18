<template>
    <div class="post">
        <h3>{{ props.title }}</h3>
        <p>{{ props.content }}</p>
        <input type="text" v-model="message">
        <button @click="handleClick">Di Hola</button>
    </div>
</template>

<script setup lang="ts">
import { defineProps, defineEmits, Ref, ref } from "vue";

const props = defineProps({
    title: {
        type: String,
        required: true,
    },
    content: {
        type: String,
        required: false,
        default: "Sin contenido"
    },
});

const emit = defineEmits(["sayHi"]);

const handleClick = () => {
    emit("sayHi", message.value)
};

let message: Ref<string> = ref("");
</script>

<style scoped>
.post {
    width: 300px;
    border-radius: 10px;
    height: 200px;
    background-color: antiquewhite;
    margin: 10px;
    padding: 10px;
}
</style>