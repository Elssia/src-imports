<template src="../html/index.html">
</template>
<script setup>
import {defineAsyncComponent,computed,ref} from 'vue'
const errLoadComponent = defineAsyncComponent(() => import('./errLoadComponent.vue'));
const test = ()=>{
  console.log("6666666")
}
let value = ref("你好")
</script>