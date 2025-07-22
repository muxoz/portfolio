<script setup>
import { cn } from '@/lib/utils';

const props = defineProps({
  class: { type: null, required: false },
});
</script>

<template>
  <div data-slot="card-footer" :class="cn('[.border-t]:pt-6 flex items-center px-6', props.class)">
    <slot />
  </div>
</template>
