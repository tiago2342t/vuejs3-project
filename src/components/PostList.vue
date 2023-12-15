<template>
    <div class="container">
        <PostDetail v-for="elm in info" :key="elm.title" :title="elm.title" :content="elm.content" @sayHi="showAlert" />
    </div>
</template>

<script setup lang="ts">
import PostDetail from './PostDetail.vue';
interface Post {
    title: string,
    content: string,
}

let info: Array<Post> = [
    {
        title: "Post 1",
        content: "Texto 1"
    },
    {
        title: "Post 2",
        content: "Texto 2"
    },
    {
        title: "Post 3",
        content: "Texto 3"
    },
    {
        title: "Post 4",
        content: "Texto 4"
    },
    {
        title: "Post 5",
        content: "Texto 5"
    },
];
function showAlert(msg: string) {
    alert(msg)
}
</script>

<style scoped>
.container {
    display: flex;
    flex-wrap: wrap;
    flex-direction: row;
    justify-content: space-around;
}
</style>