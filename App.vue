<template>
  <h1>Contador</h1>
  <CounterComposition/>
</template>

<script lang="ts" setup>
  import CounterOption from './components/CounterOption.vue';
  import CounterComposition from './components/CounterComposition.vue';
</script>

<style>
  h1{
    text-align: center;
    color: green;
  }
</style>
