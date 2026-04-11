<script setup lang="ts">
defineProps<{ url: string }>();

const unscaledSize = 'calc(100% * var(--slidev-slide-scale))';
const unscaledTransform = 'scale(calc(1 / var(--slidev-slide-scale)))';
</script>

<template>
  <div class="h-full w-full overflow-hidden">
    <div relative :style="{ width: unscaledSize, height: unscaledSize }">
      <iframe
        class="w-full h-full border-none"
        :src="url"
        :style="{
          transform: unscaledTransform,
          transformOrigin: 'top left'
        }"
      />
    </div>
  </div>
</template>