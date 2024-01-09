<template>
    

<div class="relative overflow-x-auto shadow-md sm:rounded-lg">
    <table class="w-full text-sm text-left rtl:text-right text-gray-500 dark:text-gray-400">
        <caption class="p-5 text-lg font-semibold text-left rtl:text-right text-gray-900 bg-white dark:text-white dark:bg-gray-800">
            Domains Manager
            <p class="mt-1 text-sm font-normal text-gray-500 dark:text-gray-400">Łatwo i szybko zorganizuj swoje domeny! </p>
        </caption>
        <thead class="text-xs text-gray-700 uppercase bg-gray-50 dark:bg-gray-700 dark:text-gray-400">
            <tr>
                <th scope="col" class="px-6 py-3">
                    Strona
                </th>
                <th scope="col" class="px-6 py-3">
                    Host
                </th>
                <th scope="col" class="px-6 py-3">
                    Data zakupu
                </th>
                <th scope="col" class="px-6 py-3">
                    Data zakończenia
                </th>
                <th scope="col" class="px-6 py-3">
                    <span class="sr-only">Edytuj</span>
                </th>
                <th scope="col" class="px-6 py-3">
                    <span class="sr-only">Usuń</span>
                </th>
            </tr>
        </thead>
        <tbody>
            <TableRow :domains="domains"/>
            <!-- <tr v-for="domain in domains" :key="domain.id" class="bg-white border-b dark:bg-gray-800 dark:border-gray-700">
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
            </tr> -->
            <!-- <tr class="bg-white border-b dark:bg-gray-800 dark:border-gray-700">
                <th scope="row" class="px-6 py-4 font-medium text-gray-900 whitespace-nowrap dark:text-white">
                    Microsoft Surface Pro
                </th>
                <td class="px-6 py-4">
                    White
                </td>
                <td class="px-6 py-4">
                    Laptop PC
                </td>
                <td class="px-6 py-4">
                    $1999
                </td>
                <td class="px-6 py-4 text-right">
                    <a href="#" class="font-medium text-blue-600 dark:text-blue-500 hover:underline">Edit</a>
                </td>
            </tr> -->
            <!-- <tr class="bg-white dark:bg-gray-800">
                <th scope="row" class="px-6 py-4 font-medium text-gray-900 whitespace-nowrap dark:text-white">
                    Magic Mouse 2
                </th>
                <td class="px-6 py-4">
                    Black
                </td>
                <td class="px-6 py-4">
                    Accessories
                </td>
                <td class="px-6 py-4">
                    $99
                </td>
                <td class="px-6 py-4 text-right">
                    <a href="#" class="font-medium text-blue-600 dark:text-blue-500 hover:underline">Edit</a>
                </td>
            </tr> -->
        </tbody>
    </table>
</div>

</template>

<script setup>

import { defineProps } from "vue";
import TableRow from "@/Components/Domains/TableRow.vue";

defineProps({
    domains: Array,
});
</script>