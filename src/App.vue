<template>
  <div class="flex flex-col sm:justify-center items-center p-1 sm:h-screen bg-app-bg">
    <CalendarWeek />
    <CalendarEntry />
  </div>  
</template>

<script setup>
import CalendarWeek from './components/CalendarWeek.vue';
import CalendarEntry from './components/CalendarEntry.vue';

</script>

<style>
</style>
