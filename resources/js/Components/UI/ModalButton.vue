<template>
    <fwb-button @click="emitShowModalEvent"> Open modal </fwb-button>
  </template>
  
  <script lang="ts" setup>
  import { ref } from "vue";
  
  const emitShowModal = ref(null);
  
  function emitShowModalEvent() {
    emitShowModal.value = true;
  }
  </script>