<template>
    <div v-if="show" class="fixed inset-0 bg-black opacity-50 grid place-items-center">
<div class="bg-white w-[50%]">

    <header>header</header>
    
    <div></div>
    
    <footer>footer</footer>
</div>
    </div>
</template>


<script setup>
defineProps({
    show:Boolean
})

</script>