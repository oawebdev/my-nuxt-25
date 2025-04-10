<template>
  <Table :data="data?.products" :loading="status === 'pending'"/>

</template>
<script setup lang="ts">
const { data, status, error, refresh } = await useLazyFetch(() => `https://dummyjson.com/products`, {
  //query: { param2: param1.value },
  params: {},
})
</script>