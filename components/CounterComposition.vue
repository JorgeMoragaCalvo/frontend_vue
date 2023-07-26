<template>
    <h3>{{ counter }}</h3>
    <button @click="addCounter">Incrementar</button>
</template>

<script lang="ts">
    import { defineComponent, ref } from 'vue';
    export default defineComponent({
        name: 'CounterComposition',
        setup(){
            let counter = ref(0); // ref: reactive value. Indica que el valor puede cambiar, es reactivo.
            const addCounter = () => {
                counter.value++;
                if(counter.value > 20){
                    counter.value = 0;
                }
            }
            return {counter, addCounter}
        }
    })
</script>