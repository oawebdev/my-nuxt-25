<template>
  <div>{{ a }}</div>
  <div>Dynamic</div>
</template>
<script setup lang="ts">
const route = useRouter();
let a = route.currentRoute.value.params.id
</script>