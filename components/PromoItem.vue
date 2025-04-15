<template>
  <div class="flex items-center gap-3" :data-aos="animation">
    <span class="text-xl">✨</span>
    <p class="text-lg text-gray-800">
      <slot />
    </p>
    <span v-if="rightIcon" class="text-xl">✨</span>
  </div>
</template>

<script setup lang="ts">
  defineProps({
    animation: {
      type: String,
      default: 'fade-up',
    },
    rightIcon: {
      type: Boolean,
      default: false,
    },
  });
</script>
