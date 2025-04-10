<template>
  <div>About</div>
  <ButtonPrimary :foo="test" @update="eventHandler" />
  Parent: {{test}}
<!--  {{ status }}-->
<!--  <UButton @click="refresh">Run</UButton>-->
<!--  <pre>{{products}}</pre>-->

</template>
<script setup lang="ts">
const test = ref('def');
const eventHandler = (value: string): void => {
  test.value = value
}
const param1 = ref('test');

// const { data, status, error, refresh } = await useLazyFetch(() => `https://dummyjson.com/products?parahj=${param1.value}`, {
//   query: { param2: param1.value },
//   params: {},
// })

</script>