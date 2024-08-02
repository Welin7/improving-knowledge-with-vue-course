<!--SCRIPT-->
<script setup>
    //imports
   
    //got props
    const props = defineProps(['name', 'age']);

</script>

<!--HTML-->
<template>
   <h1>Name: {{ name }}</h1>
   <h1>Age: {{ age }}</h1>
</template> 