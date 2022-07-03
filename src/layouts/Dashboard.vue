<template>
  <div class="bg-gray-800 flex text-white max-h-screen h-screen">
    <div class="w-64">
      <span class="font-semibold p-6 block opacity-90">My Dashboard</span>
      <nav class="p-6">
        <h3 class="opacity-50 uppercase font-semibold tracking-widest mb-6 text-xs">Menu</h3>
        <div class="space-y-6">
          <MenuItem :icon="HomeIcon">Discover</MenuItem>
          <MenuItem :icon="TrendingUpIcon">Trending</MenuItem>
          <MenuItem :icon="StreamingIcon">Streaming</MenuItem>
          <MenuItem :icon="PlaylistIcon">Playlist</MenuItem>
          <MenuItem :icon="BookmarkIcon">Bookmark</MenuItem>
        </div>
      </nav>
    </div>
    <div class="flex-1 h-screen relative overflow-y-auto">
      <header class="flex p-5 bg-gray-800 z-20 sticky top-0 items-center justify-between">
        <InputSearch class="w-96" />

        <div class="flex items-center">
          <div class="flex items-center space-x-3">
            <Avatar class="rounded-full overflow-hidden w-10 h-10" />
            <span>Aluizio</span>
            <ChevronDownIcon class="w-4 h-4" />
          </div>
          <BellIcon class="w-4 h-4 ml-8 opacity-50 hover:opacity-100 cursor-pointer transition duration-100" />
          <Notifications />
        </div>
      </header>

      <div class="px-5 pb-5 content">
        <h1 class="font-bold text-4xl mt-6 mb-4">Discover</h1>

        <div class="grid grid-cols-12 gap-4">
          <div class="col-span-8 h-96 rounded-3xl overflow-hidden relative">
            <div class="flex w-full h-full">
              <img 
                class="w-full object-cover"
                src="https://img.freepik.com/fotos-gratis/vista-traseira-de-adolescente-com-skate-e-copie-espaco-no-skatepark_23-2148758475.jpg?t=st=1656807318~exp=1656807918~hmac=2fb1323f30bdef97602a1c6f648149f983f4bdf3d7eb7633606cc757ccfc3745&w=996"
                alt="Placeholder"
              />
              <div class="z-10 absolute top-0 p-6 w-full h-full bottom-0">
                <h3 class="text-2xl max-w-xs text-gray-800 mt-20 font-bold">How to do basic jumpin and how to landing safely.</h3>
                <div class="absolute right-6 bottom-6 px-2 py-1 rounded-lg bg-gray-800 bg-opacity-70 text-white font-semibold">7 minutes</div>
              </div>
            </div>
          </div>

          <div class="col-span-4 h-96 rounded-3xl overflow-hidden relative">
            <div class="flex w-full h-full">
              <img 
                class="w-full object-cover"
                src="https://img.freepik.com/fotos-gratis/jovens-andando-de-skate-no-japao_23-2149331751.jpg?t=st=1656807457~exp=1656808057~hmac=66f897439481d83a4c3b7892b2f5c1829ba32948d14b5d0f723dc0c430cd01c2&w=740"
                alt="Placeholder"
              />
              <div class="z-10 absolute top-0 p-6 w-full h-full bottom-0">
                <h3 class="text-2xl max-w-xs text-gray-300 rounded-lg bg-gray-800 bg-opacity-50 mt-20 font-bold">How to do basic jumpin and how to landing safely.</h3>
                <div class="absolute right-6 bottom-6 px-2 py-1 rounded-lg bg-gray-800 bg-opacity-70 text-white font-semibold">7 minutes</div>
              </div>
            </div>
          </div>
        </div>
          <h1 class="text-2xl mt-6 mb-4">Most Watched</h1>
          <div class="grid grid-cols-4 gap-4">
            <CardItem v-for="n of 4" />
          </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
  import MenuItem from './navs/MenuItem.vue';
  import Avatar from '../components/Avatar.vue';
  import CardItem from '../components/CardItem.vue';
  import BellIcon from '../components/icons/BellIcon.vue';
  import HomeIcon from '../components/icons/HomeIcon.vue';
  import InputSearch from '../components/inputs/InputSearch.vue';
  import PlaylistIcon from '../components/icons/PlaylistIcon.vue';
  import BookmarkIcon from '../components/icons/BookmarkIcon.vue';
  import StreamingIcon from '../components/icons/StreamingIcon.vue';
  import TrendingUpIcon from '../components/icons/TrendingUpIcon.vue';
  import ChevronDownIcon from '../components/icons/ChevronDownIcon.vue';
</script>