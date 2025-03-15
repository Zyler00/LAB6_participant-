<script setup lang="ts">
import { ref } from 'vue'
import type { Participant } from '@/types'
const event = ref<Participant>()
</script>
<template>
 <div>
 <h1>{{ event.name }}</h1>
 <p>{{ event.email }}</p>
 <p>{{ event.events }}</p>
 </div>
</template>
