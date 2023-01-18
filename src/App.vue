<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <div class="wrapper">
      <nav>
        <RouterLink :to="{ name: 'event-list' }">Events</RouterLink>
        <RouterLink :to="{ name: 'about' }">About</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style></style>
