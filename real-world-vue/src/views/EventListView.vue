<script setup lang="ts">
// import TheWelcome from '../components/TheWelcome.vue'
import EventCard from '../components/EventCard.vue'
// import CategoryView from '../components/Category.vue'
import { events } from '@/events';
// import type { EventItem } from '@/type'
// import { ref } from 'vue'

</script>

<template>
  <h1>Event For Good</h1>
  <main class="events">
    <EventCard v-for="event in events" :key="event.id" :event="event"></EventCard>
  </main>
</template>

<style scoped>
.events {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
