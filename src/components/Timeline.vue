<template>
  <div class="timeline-container">
    <TimelineItem v-for="(item, i) in timelineData" :data="item" :key="i" />
  </div>
</template>

<script>
import json from '../assets/data.json'
import TimelineItem from './TimelineItem.vue'

export default {
  components: {
    TimelineItem,
  },
  data: () => ({
    timelineData: json,
  }),
}
</script>

<style></style>
