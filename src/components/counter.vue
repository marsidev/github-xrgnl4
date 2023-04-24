<template>
  <div>
    <button @click="incrementCounter">+</button>
    <span>Counter: {{ counter }}</span>
    <button @click="decrementCounter">-</button>
  </div>
</template>

<script setup lang="ts">
import { DndProvider } from 'vue3-dnd';
import { ref } from 'vue';

// Define counter as a reactive property
const counter = ref(0);

// Function to increment the counter
function incrementCounter() {
  counter.value++;
}

// Function to decrement the counter
function decrementCounter() {
  counter.value--;
}
</script>
