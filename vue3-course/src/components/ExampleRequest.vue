<!--SCRIPT-->
<script setup>
//Imports
import { onMounted, ref } from 'vue';

//vector contain the posts
let vector= ref([]);

//onMounted, call of api jsonplaceholder of posts
onMounted(() => {
    fetch('https://jsonplaceholder.typicode.com/posts')
    .then(response => response.json())
    .then(response => vector.value = response)
});


</script>

<!--HTML-->
<template>
    <h1>Resquests</h1>
    
    <table>
        <tr v-for="item in vector">
            <td>{{ item.userId }}</td>
            <td>{{ item.id }}</td>
            <td>{{ item.title }}</td>
            <td>{{ item.body }}</td>
        </tr>
    </table>
</template> 