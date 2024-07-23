<!--SCRIPT-->
<script setup>
//variable
let exibition = true;

let average = 6.5;

</script>

<!--HTML-->
<template>
    <h1 v-if="exibition"> Helo Conditional VIF!</h1>
    
    <p v-if="average >= 6">Aprooved</p>
    <p v-else-if="average >= 5">Under Examination</p>
    <p v-else>Disapproved</p>
</template>