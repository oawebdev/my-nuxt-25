<template>
  <div>About</div>
  <ButtonPrimary :foo="test" @update="eventHandler" />
  Parent: {{test}}
</template>
<script setup lang="ts">
const test = ref('def');
const eventHandler = (value: string): void => {
  test.value = value
}
</script>