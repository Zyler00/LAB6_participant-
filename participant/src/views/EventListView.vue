<script setup lang="ts">
import EventCard from '@/components/EventCard.vue'
import eventService from '@/services/EventService'
import { ref } from 'vue'
import type { Participant } from '@/types'
const events = ref<Participant[]>([])
  interface EventResponse {
 data: Participantt[]
}
eventService.getEvents().then((response:ParticipantRespose) => {
 events.value = response.data
})
</script>

<template>
 <div>
 <EventCard />
 </div>
</template>
<style scoped>
.events {
 display: flex;
 flex-direction: column;
 align-items: center;
}
</style>
