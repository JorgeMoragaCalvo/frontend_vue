<template>
    <form>
        <input type="text" v-model="inputText">
        <input type="checkbox" v-model="agree">Aceptar términos y condiciones
        <select v-model="country">
            <option value="Spain">Spain</option>
            <option value="Chile">Chile</option>
            <option value="Uk">UK</option>
        </select>
    </form>
    <h3>{{inputText}}</h3>
</template>

<script lang="ts" setup>
    import {Ref, ref } from 'vue';
    let inputText:Ref<string> = ref(''); // Ref<string> especifica el tipo de dato que se va a usar en Typescript
    let agree = ref(true);
    let country = ref('Chile');
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

<!-- Option API
    <script lang="ts">
        import {ref, defineComponent } from 'vue';
        export default defineComponent({
            data(){
                return {
                    inputText: '',
                    agree: true
                };
            }
        });
    </script>
-->