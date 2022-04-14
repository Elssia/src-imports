<template src="../html/index.html">
</template>
<script setup>
import {defineAsyncComponent,computed} from 'vue'
const errLoadComponent = defineAsyncComponent(() => import('./errLoadComponent.vue'));

</script>