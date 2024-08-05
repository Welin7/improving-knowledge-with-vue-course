<!--SCRIPT-->
<script setup>
    //imports
   
    //got props
    const props = defineProps(['name', 'age', 'city', 'citys', 'message']);

</script>

<!--HTML-->
<template>
   <h1>Name: {{ name }}</h1>
   <h1>Age: {{ age }}</h1>
   <h1>City: {{ city }}</h1>

   <ul>
        <li v-for="itens of citys">{{ itens }}</li>
   </ul>

   <button @click="message">Here Click</button>
</template> 