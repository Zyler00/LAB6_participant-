<script setup lang="ts">
import { ref } from 'vue'
import type { Event } from '@/types'
const event = ref<Event>()
</script>
<template>
 <div>
 <h1>{{ event.name }}</h1>
 <p>{{ event.email }}</p>
 <p>{{ event.events }}</p>
 </div>
</template>
