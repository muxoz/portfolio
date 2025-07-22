<script setup>
import { cn } from '@/lib/utils';

const props = defineProps({
  class: { type: null, required: false },
});
</script>

<template>
  <h3 data-slot="card-title" :class="cn('font-semibold leading-none', props.class)">
    <slot />
  </h3>
</template>
