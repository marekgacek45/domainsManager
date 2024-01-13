<template>
    <div>
        <Sidebar></Sidebar>

        <div class="p-4 md:ml-64 flex justify-center items-center h-screen">
            <div
                class="p-12   flex justify-center items-center h-full"
            >
                <create-form></create-form>
            </div>
        </div>
    </div>
</template>

<script setup>
import Sidebar from "@/Components/UI/Sidebar.vue";
import CreateForm from "@/Components/Forms/CreateForm.vue";
</script>
