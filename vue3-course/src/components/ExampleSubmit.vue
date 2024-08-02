<!--SCRIPT-->
<script setup>

//function to vlidate form
function validateForm(){
    alert('Send Form')
}

</script>

<!--HTML-->
<template>
    <form @submit="validateForm">
        <input type="submit" value="Send Form">
    </form>
</template> 