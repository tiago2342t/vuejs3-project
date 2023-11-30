<template>
    <div class="post-card">
        <h3>Título</h3>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Incidunt, quaerat cumque. Quis aliquid laborum dicta voluptatibus aut quas, doloribus dignissimos pariatur porro sapiente ipsum quasi in incidunt veritatis obcaecati fuga?</p>
        <PostButton />
    </div>
</template>

<script setup lang="ts">
import PostButton from './PostButton.vue';
</script>

<style scoped>
.post-card {
    border-radius: 15px;
    padding: 10px;
    margin: 5px;
    border: 1px solid #ccc;
}
</style>