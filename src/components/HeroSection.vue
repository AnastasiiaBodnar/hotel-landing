<script setup>
import bgImage from '../assets/background.png'
</script>

<template>
  <section class="relative h-screen w-full flex items-center justify-center text-center px-4">
    
    <div 
      class="absolute inset-0 bg-cover bg-center"
      :style="{ backgroundImage: `url(${bgImage})` }"
    ></div>

    <div class="absolute inset-0 bg-black/40"></div>

    <div class="relative z-10 text-white max-w-4xl mx-auto mt-20">
      <p class="text-lg md:text-xl font-medium tracking-widest uppercase mb-4 opacity-90">
        Welcome to
      </p>
      
      <h1 class="text-5xl md:text-7xl font-extrabold leading-tight mb-6">
        Hotel Just<span class="text-primary">Stay</span>
      </h1>
      
      <h2 class="text-2xl md:text-3xl font-semibold mb-8 opacity-90">
        Ahmedabad, India
      </h2>
      
      <p class="text-gray-200 text-lg md:text-xl max-w-2xl mx-auto mb-10 leading-relaxed">
        Lorem ipsum dolor sit, amet consectetur adipisicing elit.
        Quibusdam maxime praesentium Why did the scarecrow win 
        an award? Because he was outstanding in his field. Lorem ipsum
      </p>
      
      <div class="flex flex-col sm:flex-row gap-5 justify-center">
        <button class="bg-primary hover:bg-orange-600 text-white px-10 py-3 rounded-full font-bold text-lg transition transform hover:-translate-y-1 shadow-lg cursor-pointer">
          Book Now
        </button>
        <button class="border-2 border-white text-white hover:bg-white hover:text-gray-900 px-10 py-3 rounded-full font-bold text-lg transition cursor-pointer">
          Watch Video
        </button>
      </div>
    </div>
  </section>
</template>