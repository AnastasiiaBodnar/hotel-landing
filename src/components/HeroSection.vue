<script setup>
import bgImage from '../assets/background.png'
</script>

<template>
  <section id="home" class="relative h-screen w-full flex items-end justify-start text-left px-4 sm:px-8 md:px-10 lg:px-14 xl:px-20 pb-12">
    
    <div 
      class="absolute inset-0 bg-cover bg-center"
      :style="{ backgroundImage: `url(${bgImage})` }"
    ></div>

    <div class="absolute inset-0 bg-linear-to-r from-black/70 via-black/50 to-transparent"></div>

    <div class="relative z-10 text-white max-w-full sm:max-w-xl md:max-w-2xl lg:max-w-3xl xl:max-w-4xl">
      <p class="text-base sm:text-lg md:text-xl font-semibold leading-relaxed mb-2 text-white/90">
        Welcome to
      </p>
      
      <h1 class="text-3xl sm:text-4xl md:text-5xl lg:text-5xl xl:text-6xl font-bold leading-snug mb-4 sm:mb-5 md:mb-6">
        Hotel Just<span class="text-primary">Stay</span>
      </h1>
      
      <h2 class="text-3xl sm:text-4xl md:text-5xl lg:text-5xl xl:text-6xl font-bold mb-6 sm:mb-7 md:mb-8">
        Ahmedabad, India
      </h2>
      
      <p class="text-gray-200 text-sm sm:text-base md:text-lg lg:text-xl leading-relaxed mb-8 sm:mb-9 md:mb-10 max-w-xl lg:max-w-2xl">
        Experience luxury and comfort in the heart of Ahmedabad. 
        From elegant rooms to world-class amenities, we make every stay unforgettable.
      </p>
      
      <div class="flex flex-col sm:flex-row gap-4 sm:gap-5 justify-start">
        <button class="bg-primary hover:bg-orange-600 text-white px-8 sm:px-10 py-3 rounded-2xl font-bold text-base sm:text-lg transition transform cursor-pointer">
          Book Now
        </button>
        
        <button 
          class="group relative border-2 border-white text-white hover:bg-white hover:text-gray-900 px-8 sm:px-10 py-3 sm:py-4 rounded-2xl font-bold text-base sm:text-lg transition-all duration-300 transform hover:scale-105 hover:shadow-2xl cursor-pointer overflow-hidden"
        >
          <span class="relative z-10 flex items-center justify-center gap-2">
            Watch Video
          </span>
          <span class="absolute inset-0 bg-white transform scale-x-0 group-hover:scale-x-100 transition-transform duration-300 origin-left"></span>
        </button>
      </div>
    </div>
  </section>
</template>