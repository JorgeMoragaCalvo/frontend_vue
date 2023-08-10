<template>
  <h1>Contador</h1>
  <!--  
  <CounterComposition/>
  <CounterComposition/> cada componente es independiente -->
  <!-- <ExampleFor/> -->
  <!-- <ClassBind/> -->
  <ModelForm/>
</template>

<script lang="ts" setup>
  import ExampleSelective from './components/ExampleSelective.vue';
  import CounterComposition from './components/CounterComposition.vue';
  import ExampleFor from './components/ExampleFor.vue';
  import ClassBind from './components/ClassBind.vue';
  import ModelForm from './components/ModelForm.vue';
</script>

<style>
  h1{
    text-align: center;
    color: green;
  }
</style>
