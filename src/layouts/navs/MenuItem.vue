<template>
  <div class="flex items-center space-x-4">
    <!-- Ícone do MenuItem -->
    <div class="bg-gray-700 p-2 rounded-lg hover:bg-orange-500 cursor-pointer transition duration-100">
      <component :is="icon" class="w-4 h-4" />
    </div>
    <span>
      <!-- Nome do MenuItem -->
      <slot />
    </span>
  </div>
</template>

<script lang="ts" setup>
  import { defineProps } from "vue";
  defineProps({
    icon: { default: null },
  });
</script>