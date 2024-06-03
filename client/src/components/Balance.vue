<template>
    <h4>Your Balance</h4>
    <h1 id="balance">${{ total }}</h1>
  </template>
  
  <script setup>
  import { defineProps } from 'vue';
  
  // Define props recieved by the Balance component
  const props = defineProps({
    total: {
      type: Number, // Specify that prop 'total' expects a number value
      required: true, //Make 'toatal' prop mandatory
    },
  });
  </script>