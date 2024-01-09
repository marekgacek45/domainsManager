<template>
    

<tr v-for="domain in domains" :key="domain.id" class="bg-white border-b dark:bg-gray-800 dark:border-gray-700">
    <th scope="row" class="px-6 py-4 font-medium text-gray-900 whitespace-nowrap dark:text-white">
        <a :href="domain.siteUrl">{{domain.name}}</a>
    </th>
    <td class="px-6 py-4">
        <a :href="domain.hostUrl">{{domain.host}}</a>
    </td>
    <td class="px-6 py-4">
        {{domain.start_date}}
    </td>
    <td class="px-6 py-4">
        {{domain.end_date}}
    </td>
    <td class="px-6 py-4 text-right">
        <a href="#" class="font-medium text-blue-600 dark:text-blue-500 hover:underline">Edit</a>
    </td>
</tr>

</template>

<script setup>
import { defineProps } from "vue";
defineProps({
    domains: Array,
});
</script>