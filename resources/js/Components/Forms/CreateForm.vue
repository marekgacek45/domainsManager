<template>
    <form @submit.prevent="form.post('/domain')" class="max-w-md mx-auto">
        <form-field>
            <form-label :forHtml="name">Nazwa</form-label>
            <form-input v-model="form.name" id="name" required />
        </form-field>
        <form-field>
            <form-label :forHtml="siteUrl">Adres strony</form-label>
            <form-input v-model="form.site_url" id="siteUrl" />
        </form-field>
        <form-field>
            <form-label :forHtml="host">Host</form-label>
            <form-input v-model="form.host" id="host" />
        </form-field>
        <form-field>
            <form-label :forHtml="hostUrl">Adres Hosta</form-label>
            <form-input v-model="form.host_url" id="hostUrl" />
        </form-field>
        <form-field>
            <form-label :forHtml="startDate">Data Zakupu</form-label>
            <form-input
                v-model="form.start_date"
                id="startDate"
                type="date"
                required
            />
        </form-field>
        <form-field>
            <form-label :forHtml="endDate">Data Zakończenia</form-label>
            <form-input
                v-model="form.end_date"
                id="endDate"
                type="date"
                required
            />
        </form-field>

        <button
            type="submit"
            class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm w-full sm:w-auto px-5 py-2.5 text-center dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
        >
            Dodaj
        </button>
    </form>
</template>

<script setup>
import FormField from "@/Components/UI/FormField.vue";
import FormLabel from "@/Components/Forms/Label.vue";
import FormInput from "@/Components/Forms/Input.vue";

import { useForm } from "@inertiajs/vue3";

const form = useForm({
    name: "",
    site_url: "",
    host: "",
    host_url: "",
    start_date: null,
    end_date: null,
});
</script>
