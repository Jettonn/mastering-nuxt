<template>
  <iframe
    width="560"
    height="315"
    :src="`https://player.vimeo.com/video/${props.videoId}`"
    frameborder="0"
    title="Video player"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen
  />
</template>

<script setup lang="ts">
const props = defineProps({
  videoId: {
    type: Number,
    required: true,
  },
});
</script>
