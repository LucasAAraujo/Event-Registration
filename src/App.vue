<template>
  <main class="container mx-auto my-8 space-y-8">
    <h1 class="text-4xl font-medium">Event Booking App</h1> 
    <h2 class="text-2xl font-medium">All Events</h2>
    <section class="grid grid-cols-2 gap-8">
      <EventCard  v-for="i in 6" :key="i" 
      title="Vue Conference 2024" when="21-09-2024" description="Conference about Vue and JavaScript" 
      @register="console.log('Registered!')"/>
    </section>
    <h2 class="text-2xl font-medium">Your Bookings</h2>
  </main>
</template>


<script setup>
import EventCard from '@/components/EventCard.vue';
</script>