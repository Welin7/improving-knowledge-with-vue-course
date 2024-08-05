<!--
    Props: properties:
    - The use of props provides communication between components, 
      we can send static information, variables and functions    
-->

<!--SCRIPT-->
<script setup>
    //imports
    import Props2 from "./ExampleProps2.vue";

    //variables
    let city = 'Poços de Caldas';
    let citys = ['Rio de Janeiro', 'Belo Horizonte', 'Bahia', 'São Paulo', 'Pará'];

    //function
    function Message(){
        alert('Create function in component: ExampleProps1');
    }
         
</script>

<!--HTML-->
<template>
    <Props2 name ="well" age="15" :city="city" :citys="citys" :message="Message"></Props2>
</template> 