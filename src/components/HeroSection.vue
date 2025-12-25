<script setup>
import bgImage from '../assets/background.png'
</script>

<template>
  <section class="relative h-screen w-full flex items-center justify-start text-left pl-14">
    
    <div 
      class="absolute inset-0 bg-cover bg-center"
      :style="{ backgroundImage: `url(${bgImage})` }"
    ></div>

    <div class="absolute inset-0 bg-linear-to-r from-black/70 to-black/40"></div>

    <div class="relative z-10 text-white max-w-4xl mr-20 -mb-50">
      <p class=" text-xl font-semibold leading-relaxed mb-2 text-white/90">
        Welcome to
      </p>
      
      <h1 class="text-5xl font-bold leading-snug mb-6">
        Hotel Just<span class="text-primary">Stay</span>
      </h1>
      
      <h2 class="text-5xl font-bold mb-8">
        Ahmedabad, India
      </h2>
      
      <p class="text-gray-200 text-xl max-w-2xl mb-10 leading-relaxed">
        Lorem ipsum dolor sit, amet consectetur adipisicing elit.
        Quibusdam maxime praesentium Why did the scarecrow win 
        an award? Because he was outstanding in his field. Lorem ipsum
      </p>
      
      <div class="flex flex-col sm:flex-row gap-5 justify-start">
        <button class="bg-primary hover:bg-orange-600 text-white px-10 py-3 rounded-2xl font-bold text-lg transition transform cursor-pointer">
          Book Now
        </button>
        <button class="border-2 border-white text-white hover:bg-white hover:text-gray-900 px-10 py-3 rounded-2xl font-bold text-lg transition cursor-pointer">
          Watch Video
        </button>
      </div>
    </div>
  </section>
</template>