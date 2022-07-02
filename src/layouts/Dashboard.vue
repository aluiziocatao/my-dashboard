<template>
  <div class="bg-gray-800 flex text-white max-h-screen h-screen">
    <div class="w-64">
      <span class="font-semibold p-6 block opacity-90">My Dashboard</span>
      <nav class="p-6">
        <h3 class="opacity-50 uppercase font-semibold tracking-widest mb-6 text-xs">Menu</h3>
        <div class="space-y-6">
          <MenuItem />
        </div>
      </nav>
    </div>
    <div class="flex-1 border-red-500">
      Content
    </div>
  </div>
</template>

<script setup lang="ts">
  import MenuItem from '../layouts/navs/ManuItem.vue';
</script>