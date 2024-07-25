<!--SCRIPT-->
<script setup>

//import ref
import { ref } from 'vue';

//variable
let name = ref('');

</script>

<!--HTML-->
<template>
    <input type="text" v-model="name">
    <p>{{ name }}</p>
</template> 