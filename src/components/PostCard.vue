<template>
    <div class="post-card">
        <h3>Titulo</h3>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque debitis non odio, molestias cum ullam corporis similique ipsa excepturi sapiente iste eos autem perspiciatis possimus cupiditate quibusdam soluta eaque voluptate.</p>
        <PostButton />
    </div>
</template>

<script lang="ts" setup>
import PostButton from "./PostButton.vue";
</script>

<style scoped>
.post-card {
    border-radius: 15px;
    padding: 10px;
    margin: 5px;
    border: 1px solid #ccc;
}
</style>