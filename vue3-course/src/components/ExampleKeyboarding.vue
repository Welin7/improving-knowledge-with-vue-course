<!--SCRIPT-->
<script setup>

//function
function Message(){
    alert('Executing the function')
}

</script>

<!--HTML-->
<template>
    <input type="text" @keyup.enter="Message">
</template> 