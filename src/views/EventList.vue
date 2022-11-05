<script setup lang="ts">
import EventCard from '@/components/EventCard.vue';

const events = [
  {
    id: 1,
    category: 'animal welfare',
    title: 'cat adoption day',
    location: 'meow town',
    description: 'Find your new feline friend at this event',
    date: 'January 28, 2022'
  },
  {
    id: 2,
    category: 'animal welfare',
    title: 'dog adoption day',
    location: 'wuff town',
    description: 'Find your new friend at this event',
    date: 'January 29, 2022'
  },
  {
    id: 3,
    category: 'animal welfare',
    title: 'bird adoption day',
    location: 'chirp town',
    description: 'Find your new friend at this event',
    date: 'January 30, 2022'
  },
]
  
</script>

<template>
  <main>
    <h1>Welcome</h1>
    <ul>
      <li v-for="event in events" :key="event.id">
        <EventCard :event="event"></EventCard>
      </li>
    </ul>
  </main>
</template>