<!--SCRIPT-->
<script setup>

//variable
let validation = false;

</script>

<!--CSS-->
<style>
    .ok{color: aqua;}
    .fail{color: red;}
</style>

<!--HTML-->
<template>
    <p :class="validation ? 'ok' : 'fail'">Using directive class</p>
</template> 