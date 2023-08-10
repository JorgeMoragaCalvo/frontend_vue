<template>
    <form>
        <input type="text" v-model="inputText">
    </form>
    <h3>{{inputText}}</h3>
</template>

<script lang="ts" setup>
    import {Ref, ref } from 'vue';
    let inputText:Ref<string> = ref(''); // Ref<string> especifica el tipo de dato que se va a usar en Typescript
</script>

<style scoped>

</style>

<!-- Composition API
    <script lang="ts">
        import {ref, defineComponent } from 'vue';
        export default defineComponent({
            setup(){
                let inputText = ref('');
                return {inputText};
            }
        });
    </script>
-->