<template>
  <div>sasadasd</div>
  <ButtonPrimary v-model="amount" text="Count"/>
  Parent: {{amount}}
  <button @click="amount--">--</button>
  <NuxtPage/>
</template>
<script setup lang="ts">
const amount = ref(10);
</script>