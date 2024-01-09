<template>
    
      

        <Table :domains="domains" />
    
</template>

<script setup>
import { defineProps } from "vue";

import Table from "@/Components/Domains/Table.vue";

defineProps({
    domains: Array,
});
</script>
