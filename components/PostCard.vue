<template>
    <div class="post-card">
        <h3>Titulo</h3>
        <p>Netlify is a remote-first cloud computing company that offers a development platform that includes build, 
            deploy, and serverless backend services for web applications and dynamic websites.</p>
        <PostButton/>
    </div>
</template>

<script lang="ts" setup>
    import PostButton from './PostButton.vue';
</script>

<style scoped>
    .post-card{
        border-radius: 15px;
        padding: 10px;
        margin: 5px;
        border: 1px solid #ccc;
    }
</style>

