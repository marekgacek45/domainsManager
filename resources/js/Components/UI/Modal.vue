<template>
    <div v-if="show" class="fixed top-0 right-0 bottom-0 left-0 md:left-64 bg-black opacity-50 grid place-items-center" >
<div class="bg-white w-[50%]">

    <header>header</header>
    
    <div></div>
    
    <footer>

        <button @click="$emit('close')">close</button>
    </footer>
</div>
    </div>
</template>


<script setup>
defineProps({
    show:Boolean
})

</script>