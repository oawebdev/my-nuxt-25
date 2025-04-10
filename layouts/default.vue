<template>
  <div>
    <UNavigationMenu color="neutral" :items="items" class="w-full" />
    <slot />
  </div>
</template>

<script setup lang="ts">
const items = ref([
  [
    {
      label: 'Home',
      icon: 'i-ix-about',
      to: '/'
    },
    {
      label: 'About',
      icon: 'i-ix-about',
      to: '/about'
    },
    {
      label: 'Products',
      icon: 'i-lucide-box',
      to: '/products',
    }
  ],
  [
    {
      label: 'contacts',
      icon: 'i-simple-icons-github',
      to: '/contacts',
    }
  ]
])
</script>


