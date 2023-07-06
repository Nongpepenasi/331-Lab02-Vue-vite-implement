<script setup lang="ts">
import Category from '../components/Category.vue'
import { events } from '@/events';
</script>

<template>
  <div class="category">
    <h1>This is a categories page</h1>
    <!-- <Category></Category> -->
    <div class="category">
      <Category v-for="event in events" :key="event.id" :event="event"></Category>
    </div>
  </div>
</template>

<style>
.category {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: right;
}
</style>
