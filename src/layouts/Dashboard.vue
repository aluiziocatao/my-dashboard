<template>
  <div class="bg-gray-800 flex text-white max-h-screen h-screen">
    <div class="w-64">
      <span class="font-semibold p-6 block opacity-90">My Dashboard</span>
      <nav class="p-6">
        <h3 class="opacity-50 uppercase font-semibold tracking-widest mb-6 text-xs">Menu</h3>
        <div class="space-y-6">
          <MenuItem :icon="HomeIcon">Discover</MenuItem>
          <MenuItem :icon="TrendingUpIcon">Trending</MenuItem>
          <MenuItem :icon="HomeIcon">Discover</MenuItem>
          <MenuItem :icon="TrendingUpIcon">Trending</MenuItem>
          <MenuItem :icon="HomeIcon">Discover</MenuItem>
          <MenuItem :icon="TrendingUpIcon">Trending</MenuItem>
        </div>
      </nav>
    </div>
    <div class="flex-1 p-5">
      <header class="flex items-center justify-between">
        <InputSearch class="w-96" />

        <div class="flex items-center">
          <div class="flex items-center space-x-3">
            <div class="w-10 h-10">
              <Avatar class="rounded-full" />
            </div>
            <span>Aluizio</span>
            <ChevronDownIcon class="w-4 h-4" />
          </div>
          <BellIcon class="w-4 h-4 ml-8 opacity-50 hover:opacity-100 cursor-pointer transition duration-100" />
          <Notifications />
        </div>
      </header>
    </div>
  </div>
</template>

<script setup lang="ts">
  import MenuItem from './navs/MenuItem.vue';
  import Avatar from '../components/Avatar.vue';
  import BellIcon from '../components/icons/BellIcon.vue';
  import HomeIcon from '../components/icons/HomeIcon.vue';
  import InputSearch from '../components/inputs/InputSearch.vue';
  import TrendingUpIcon from '../components/icons/TrendingUpIcon.vue';
  import ChevronDownIcon from '../components/icons/ChevronDownIcon.vue';
</script>