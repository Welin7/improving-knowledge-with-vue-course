<!--SCRIPT-->
<script setup>
//variable
let names = ['Joao', 'Maria', 'Jose', 'Carolina', 'Lavinia', 'Davi'];

</script>

<!--HTML-->
<template>
    <ul>
        <li v-for="name in names">{{name}}</li>
    </ul>
</template>