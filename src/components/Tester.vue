<script lang="ts" setup>
const props = defineProps<{lastName: string}>()
</script>

<template>
  <h3>Props rec'd: {{ props.lastName }}</h3>
</template>
