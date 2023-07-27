<template>
    <ul>
        <li v-for="(country, index) in countries" v-bind:key="index">{{country}}</li>
        <!-- v-bind:key == :key -->
    </ul>
</template>

<script lang="ts" setup>
    import {Ref, ref} from 'vue';
    let countries:Ref<Array<string>> = ref(['Mexico', 'Colombia', 'Peru', 'Chile', 'Argentina']); //typescript
    //para el caso de JS let countries = ref(['Mexico', 'Colombia', 'Peru', 'Chile', 'Argentina']);
</script>

<style scoped>

</style>
