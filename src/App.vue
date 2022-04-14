<script setup>

import {defineAsyncComponent,computed} from 'vue'
const asyncComponent= defineAsyncComponent(() => import('./components/asyncComponent.vue'));


 const getComponent = computed(() => {

    return asyncComponent;

});
</script>

<template >
<component :is="getComponent"></component>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
