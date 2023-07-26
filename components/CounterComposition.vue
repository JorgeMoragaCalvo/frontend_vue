<template>
    <h3>{{ counter }}</h3>
    <button @click="addCounter">Incrementar</button>
</template>

<script lang="ts" setup>
    import { Ref, ref } from 'vue'; //Tipado en TS    
    let counter:Ref = ref(0); // ref: reactive value. Indica que el valor puede cambiar, es reactivo.
    const addCounter = ():void => {
            counter.value++;
            if(counter.value > 20){
                counter.value = 0;
            }
        }
</script>