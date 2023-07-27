<template>
    <ul>
        <li v-for="(country, index) in countries" v-bind:key="index">{{country.code}}</li>
        <!-- v-bind:key == :key -->
    </ul>
</template>

<script lang="ts" setup>
    import {Ref, ref} from 'vue';
    interface ICountry{
        code: string;
        name: string;
    }
    //en Typescript es necesario definir el tipo de dato de la variable
    //para el caso de JS no es necesario. En este caso se define un array de objetos
    //llamados ICountry
    let countries:Ref<Array<ICountry>>= ref([
        {
            code: "cl",
            name: "Chile"
        },
        {
            code: "ar",
            name: "Argentina"
        },
        {
            code: "co",
            name: "Colombia"
        },
        {
            code: "pe",
            name: "Peru"
        },
        {
            code: "mx",
            name: "Mexico"
        },
    ]); //typescript
    //para el caso de JS let countries = ref(['Mexico', 'Colombia', 'Peru', 'Chile', 'Argentina']);
</script>

<style scoped>

</style>
