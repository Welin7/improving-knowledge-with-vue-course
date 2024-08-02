<!--
    Lifecycle: are actions can happened in tree process of component:
    - before of criation
    - during criation
    - after criation
-->

<!--SCRIPT-->
<script setup>
    //imports
    import { onMounted, ref } from 'vue';

    //Variable
    let text = ref('Hello Word');

    //Lifecycle onMounted
    onMounted(() => {
        setTimeout(() => {
            text.value = 'Modify text';
        }, 3000);
    });
</script>

<!--HTML-->
<template>
    <h1>{{ text }}</h1>
</template> 