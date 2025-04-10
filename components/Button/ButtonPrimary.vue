<template>
  <UButton @click="myclick" variant="outline">
    test {{count}}
  </UButton>

  <div>Props: {{ foo }}</div>
</template>
<script setup lang="ts">
const count = defineModel({default:0});
const props = defineProps<{
  foo: string
  bar?: number|null
}>()

const emit = defineEmits<{
  (e: 'change'): void
  (e: 'update', value: string): void
}>()


const myclick = () => {
  count.value++
  emit('update', 'text')
}
</script>
<style lang="postcss" scoped>
.test {
  @apply bg-amber-200 p-4;
}
</style>