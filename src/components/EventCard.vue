<script setup>
defineProps({
  event: {
    type: Object,
    required: true,
  },
})
</script>

<template>
  <RouterLink :to="{ name: 'event-details', params: { id: event.id } }">
    <div class="event-card">
      <h2>{{ event.title }}</h2>
      <span>@{{ event.time }} on {{ event.date }}</span>
    </div>
  </RouterLink>
</template>

<style scoped>
.event-card {
  background-color: #f9f9f9;
}
</style>
