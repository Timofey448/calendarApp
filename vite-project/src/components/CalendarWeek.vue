<template>
  <div class="flex flex-wrap lg:flex-nowrap justify-center sm:mx-auto mb-16">
    <CalendarDay      
      v-for="day in sharedState.data"
      :key="day.id"
      :day="day"      
    />
  </div>  
</template>

<script>
import { store } from '../store';
import CalendarDay from './CalendarDay.vue';

export default {
  name: "CalendarWeek",
  data() {
    return {
      sharedState: store.state // объект  - data: seedData
    }
  },
  components: {
    CalendarDay
  }
}
</script>

