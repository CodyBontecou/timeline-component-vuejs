<template>
  <div class="timeline-item">
    <div class="timeline-item-content">
      <span class="tag" :style="{ background: `${data.category.color}` }">
        {{ data.category.tag }}
      </span>
      <time>{{ data.date }}</time>
      <p>{{ data.text }}</p>
      <a
        v-if="data.link"
        :href="data.link.url"
        target="_blank"
        rel="noopener noreferrer"
      >
        {{ data.link.text }}
      </a>
      <span class="circle" />
    </div>
  </div>
</template>

<script>
export default {
  props: {
    data: {
      type: Object,
      required: true,
    },
  },
}
</script>

<style></style>
