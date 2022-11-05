<script setup lang="ts">
  defineProps<{
    event: any;
  }>()
</script>

<template>
  <div>
    <span>@{{event.date}}</span>
  </div>
</template>