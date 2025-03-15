<script setup lang="ts"></script>

<template>
 <RouterLink to="participant">
<div class="event-card">
<h2>{{ event.name }}</h2>
<p>{{ event.events }}</p>
<span>{{ event.email }}</span>
</div>
</RouterLink>
</template>

<style scoped>
.event-card {
 padding: 20px;
 width: 250px;
 cursor: pointer;
 border: 1px solid #39495c;
 margin-bottom: 18px;
}
.event-card:hover {
 transform: scale(1.01);
 box-shadow: 0 3px 12px 0 rgba(0, 0, 0, 0.2);
}
</style>
