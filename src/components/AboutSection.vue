<script setup>
import aboutImage from '../assets/about.png'
</script>

<template>
  <section id="about" class="py-20 px-20">
    <div class="max-w-7xl mx-auto grid grid-cols-2 gap-12 items-center">
      
      <div class="relative">
        <div class="rounded-3xl overflow-hidden shadow-2xl">
          <img 
            :src="aboutImage" 
            alt="About JustStay" 
            class="w-full h-full object-cover"
          >
        </div>
      </div>

      <div>
        <p class="text-title text-sm font-semibold mb-2 tracking-wide">
          — About Us — 
        </p>
        
        <h2 class="text-heading text-5xl font-bold mb-6">
          History of Just<span class="text-primary">Stay</span>
        </h2>
        
        <p class="text-text text-base leading-relaxed mb-4">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Doloremque 
          assumenda incidunt in cum. Fugiat repellat cumque deserunt, at ipsum et 
          iure explicabo perferendis. Why do we press harder on the remote control 
          when we know the batteries are flat?
        </p>
        
        <p class="text-muted text-sm leading-relaxed mb-8">
          Autam temporibus, neque voluptas officiis molestiae. At vero eos et 
          accusamus et iusto odio dignissimos ducimus, qui blanditiis praesentium. 
          Listening to a never-ending sales pitch, right? And why is it that when 
          we're stuck in traffic, the other lane always seems to be moving faster? 
          you need a pun, it's always out of ink?
        </p>
        
        <button class="bg-primary text-white px-8 py-3 rounded-2xl font-bold text-base transition cursor-pointer">
          Read More
        </button>
      </div>
      
    </div>

    <div class="max-w-7xl mx-auto grid grid-cols-2 gap-12 items-center mt-32">
      
      <div>
        <h2 class="text-heading text-5xl font-bold mb-6">
          Why Choose us?
        </h2>
        
        <p class="text-text text-base leading-relaxed mb-4">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Doloremque 
          assumenda incidunt in cum. Fugiat repellat cumque deserunt, at ipsum et 
          iure explicabo perferendis. Why do we press harder on the remote control 
          when we know the batteries are weak?
        </p>
        
        <p class="text-muted text-sm leading-relaxed mb-8">
          Autam temporibus, neque voluptas officiis molestiae. At vero eos et 
          accusamus et iusto odio dignissimos ducimus. And why is it that one time 
          you need a pun, it's always out of ink?
        </p>
        
        <button class="bg-primary text-white px-8 py-3 rounded-2xl font-bold text-base transition cursor-pointer">
          Read More
        </button>
      </div>

      <div class="relative">
        <div class="rounded-3xl overflow-hidden shadow-2xl">
          <img 
            :src="aboutImage" 
            alt="Why Choose Us" 
            class="w-full h-full object-cover"
          >
        </div>
      </div>
      
    </div>
  </section>
</template>