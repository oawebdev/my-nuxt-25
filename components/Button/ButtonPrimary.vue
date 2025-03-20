<template>
  <button @click="count++">
    test {{count}}
  </button>
</template>
<script setup lang="ts">
const count = defineModel({default:0});
const props = defineProps({
  text
})

</script>