<template>
  <div>
    {{ date }}
  </div>
</template>
<script lang="ts" setup>
const date = ref()
//is server side
if (process.server) {
  date.value = new Date()
}
</script>