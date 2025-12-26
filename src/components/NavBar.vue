<script setup>
import { ref } from 'vue'

const isMenuOpen = ref(false)

const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value
}
</script>

<template>
  <nav class="text-white py-4 px-4 sm:px-8 flex justify-between items-center absolute w-full top-0 z-50">
    
    <div class="text-xl sm:text-2xl font-bold">
      Just<span class="text-primary">Stay</span>
    </div>

    <ul class="hidden md:flex gap-6 lg:gap-8 font-medium">
      <li><a href="#home" class="hover:text-primary transition">Home</a></li>
      <li><a href="#about" class="hover:text-primary transition">About</a></li>
      <li><a href="#services" class="hover:text-primary transition">Services</a></li>
      <li><a href="#rooms" class="hover:text-primary transition">Rooms</a></li>
      <li><a href="#contact" class="hover:text-primary transition">Contact</a></li>
    </ul>

    <div class="hidden md:flex items-center gap-2 font-medium text-lg">
      <span class="text-primary font-bold cursor-default">EN</span>
      <span class="text-white">|</span>
      <a href="/" class="text-white transition cursor-pointer">UA</a>
    </div>


    <button 
      @click="toggleMenu" 
      class="md:hidden relative z-50 w-8 h-8"
    >
      <div class="flex flex-col gap-1.5 items-end">
        <span 
          class="block h-0.5 bg-white transition-all duration-300"
          :class="isMenuOpen ? 'w-8 rotate-45 translate-y-2' : 'w-8'"
        ></span>
        <span 
          class="block h-0.5 bg-white transition-all duration-300"
          :class="isMenuOpen ? 'w-8 opacity-0' : 'w-8'"
        ></span>
        <span 
          class="block h-0.5 bg-white transition-all duration-300"
          :class="isMenuOpen ? 'w-8 -rotate-45 -translate-y-2' : 'w-8'"
        ></span>
      </div>
    </button>

    <div 
      class="fixed inset-0 bg-black/98 backdrop-blur-xl flex items-center justify-center transition-all duration-500 md:hidden"
      :class="isMenuOpen ? 'opacity-100 visible' : 'opacity-0 invisible'"
    >
      <ul class="flex flex-col gap-8 text-center font-medium text-2xl">
        <li 
          v-for="(item, index) in ['Home', 'About', 'Services', 'Rooms', 'Contact']" 
          :key="item"
          class="transition-all duration-500 delay-75"
          :class="isMenuOpen ? 'translate-y-0 opacity-100' : 'translate-y-10 opacity-0'"
          :style="{ transitionDelay: `${index * 100}ms` }"
        >
          <a 
            :href="`#${item.toLowerCase()}`" 
            @click="toggleMenu" 
            class="hover:text-primary transition"
          >
            {{ item }}
          </a>
        </li>
        
        <li class="mt-8 flex items-center justify-center gap-4 text-xl">
          <span class="text-primary font-bold">EN</span>
          <span>|</span>
          <a href="/" class="hover:text-primary transition">UA</a>
        </li>
      </ul>
    </div>
  </nav>
</template>