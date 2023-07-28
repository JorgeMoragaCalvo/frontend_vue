<template>
  <h1>Contador</h1>
  <!--  
  <CounterComposition/>
  <CounterComposition/> cada componente es independiente -->
  <!-- <ExampleFor/> -->
  <ClassBind/>
</template>

<script lang="ts" setup>
  import ExampleSelective from './components/ExampleSelective.vue';
  import CounterComposition from './components/CounterComposition.vue';
  import ExampleFor from './components/ExampleFor.vue';
  import ClassBind from './components/ClassBind.vue';
</script>

<style>
  h1{
    text-align: center;
    color: green;
  }
</style>
