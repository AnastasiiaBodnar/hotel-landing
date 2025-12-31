<script setup>
import aboutImage from '../assets/about.png'
</script>

<template>
  <section id="about" class="pt-5">

    <div class="px-4 sm:px-6 md:px-8 lg:px-10 flex justify-center mb-10">
      <p class="text-title text-xs sm:text-sm font-semibold tracking-wide">
        — About Us — 
      </p>
    </div>
        
    <div class="px-4 sm:px-6 md:px-8 lg:px-10 max-w-7xl mx-auto grid grid-cols-1 lg:grid-cols-2 gap-6 md:gap-8 lg:gap-12 items-start mt-10">
      
      <div class="relative">
        <img 
          :src="aboutImage" 
          alt="About JustStay" 
          class="w-full md:w-4/5 md:mx-auto lg:w-full lg:max-h-70 h-auto rounded-2xl object-cover"
          style="outline: 1px solid #c9c9c9; outline-offset: 10px;"
        >
      </div>

      <div>

        <h2 class="text-heading text-2xl sm:text-3xl lg:text-4xl font-bold mb-4">
          History of Just<span class="text-primary">Stay</span>
        </h2>
        
        <p class="text-text text-sm sm:text-base lg:text-sm font-medium leading-relaxed mb-4">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Doloremque 
          assumenda incidunt id cum. Fugiat repellat cumque delectus, at ipsum ad 
          iure explicabo perferendis. If you're still reading this, congrats, you're 
          officially a masochist.
        </p>
        
        <p class="text-muted text-xs sm:text-sm lg:text-xs leading-relaxed mb-4">
          Autem temporibus, neque voluptas officiis molestiae. At vero eos et 
          accusamus et iusto odio dignissimos ducimus. But hey, at least you're not stuck in traffic, 
          or worse, listening to a never-ending sales pitch, right?
        </p>
        
        <button class="bg-white text-primary px-6 sm:px-8 py-2.5 sm:py-3 rounded-2xl font-bold text-sm sm:text-base transition cursor-pointer border-2 border-primary">
          Read More
        </button>
      </div>
      
    </div>

    <div class="px-4 sm:px-6 md:px-8 lg:px-10 max-w-7xl mx-auto grid grid-cols-1 lg:grid-cols-2 gap-6 md:gap-8 lg:gap-12 items-start mt-8">
      
      <div class="order-2 lg:order-1">
        <h2 class="text-heading text-2xl sm:text-3xl lg:text-4xl font-bold mb-4">
          Why Choose us?
        </h2>
        
        <p class="text-text text-sm sm:text-base lg:text-sm font-medium leading-relaxed mb-4">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Doloremque 
          assumenda incidunt in cum. Fugiat repellat cumque deserunt, at ipsum et 
          iure explicabo perferendis. 
        </p>
        
        <p class="text-muted text-xs sm:text-sm lg:text-xs leading-relaxed mb-4">
          Autam temporibus, neque voluptas officiis molestiae. At vero eos et 
          accusamus et iusto odio dignissimos ducimus. And why is it that one time 
          you need a pun, it's always out of ink?
        </p>
        
        <button class="bg-white text-primary px-6 sm:px-8 py-2.5 sm:py-3 rounded-2xl font-bold text-sm sm:text-base transition cursor-pointer border-2 border-primary">
          Read More
        </button>
      </div>

      <div class="relative order-1 lg:order-2">
        <img 
          :src="aboutImage" 
          alt="About JustStay" 
          class="w-full md:w-4/5 md:mx-auto lg:w-full lg:max-h-70 h-auto rounded-2xl object-cover"
          style="outline: 1px solid #c9c9c9; outline-offset: 10px;"
        >
      </div>
    </div>

    <div class="w-full bg-primary py-6 sm:py-8 lg:py-4 px-4 sm:px-6 lg:px-8 mt-12">
      <div class="grid grid-cols-2 lg:grid-cols-4 gap-4 sm:gap-6 lg:gap-8">
        <div class="text-center">
          <h3 class="text-white text-2xl sm:text-3xl lg:text-4xl font-bold mb-2">8</h3>
          <p class="text-white text-xs sm:text-sm font-medium">Years of Service</p>
        </div>
        <div class="text-center">
          <h3 class="text-white text-2xl sm:text-3xl lg:text-4xl font-bold mb-2">459</h3>
          <p class="text-white text-xs sm:text-sm font-medium">Sq. Meter Area</p>
        </div>
        <div class="text-center">
          <h3 class="text-white text-2xl sm:text-3xl lg:text-4xl font-bold mb-2">50</h3>
          <p class="text-white text-xs sm:text-sm font-medium">Nice Rooms</p>
        </div>
        <div class="text-center">
          <h3 class="text-white text-2xl sm:text-3xl lg:text-4xl font-bold mb-2">3786</h3>
          <p class="text-white text-xs sm:text-sm font-medium">Happy Visitors</p>
        </div>
      </div>
    </div>

  </section>
</template>