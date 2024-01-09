<template>
    <div>
        <Sidebar></Sidebar>

        <div class="p-4 md:ml-64">
            <div
                class="p-4 border-2 border-gray-200 border-dashed rounded-lg dark:border-gray-700"
            >
                <Table :domains="domains"></Table>
            </div>
        </div>
    </div>
</template>

<script setup>
import { onMounted } from "vue";
import { initFlowbite } from "flowbite";
import { defineProps } from "vue";
import "flowbite";

onMounted(() => {
    initFlowbite();
});

import Table from "@/Components/Domains/Table.vue";
import Sidebar from "@/Components/UI/Sidebar.vue";

defineProps({
    domains: Array,
});
</script>
