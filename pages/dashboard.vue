<script lang="ts" setup>

</script>

<template>
  <div>sadasd {{ count }}</div>
</template>
<script setup lang="ts">
const config = useRuntimeConfig();
const data = $fetch(`${config.public.apiBase}/posts`);
console.log(data)
definePageMeta({
  layout: 'dashboard'
});


</script>
