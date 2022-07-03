<template>
  <div class="bg-black bg-opacity-20 rounded-3xl overflow-hidden">
    <div class="header">
      <div class="h-32 w-full flex">
        <img 
          class="w-full h-full object-cover"
          src="https://img.freepik.com/fotos-gratis/feche-os-pes-no-skate_23-2149267194.jpg?t=st=1656824203~exp=1656824803~hmac=d8e1da77eacedd538434893b96302a34f943949b230c268055636d4a828262fb&w=996" 
          alt="Imagem de Card">
      </div>
    </div>

    <div class="body relative p-5">
      <Avatar class="absolute right-2 -top-5 w-12 h-12 rounded-full overflow-hidden" />
      <h5 class="text-xs mb-2 opacity-50">
        Andy William 
        <div class="w-2 h-2 inline-block ml-2 rounded-full bg-green-400"></div>
      </h5>
      <p>Basic how to ride your skateboard comfortly</p>
      <div class="text-xs flex items-center space-x-2 opacity-50 mt-3">
        <span>53k views</span>
        <div class="w-1 h-1 rounded-full bg-gray-300"></div>
        <span>2 weeks ago</span>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
  import Avatar from './Avatar.vue';
</script>