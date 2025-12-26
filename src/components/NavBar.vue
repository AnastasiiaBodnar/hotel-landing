<script setup>
</script>

<template>
  <nav class=" text-white py-4 px-8 flex justify-between items-center absolute w-full top-0 z-50">
    
    <div class="text-2xl font-bold ">
      Just<span class="text-primary">Stay</span>
    </div>

    <ul class="hidden md:flex gap-8 font-medium">
      <li><a href="#home" class="hover:text-primary transition">Home</a></li>
      <li><a href="#about" class="hover:text-primary transition">About</a></li>
      <li><a href="#services" class="hover:text-primary transition">Services</a></li>
      <li><a href="#rooms" class="hover:text-primary transition">Rooms</a></li>
      <li><a href="#contact" class="hover:text-primary transition">Contact</a></li>
    </ul>

    <div class="flex items-center gap-2 font-medium text-lg">
      <span class="text-primary font-bold cursor-default">EN</span>
      
      <span class="text-white">|</span>
      
      <a href="/" class="text-white transition cursor-pointer" title="Switch to Ukrainian">
        UA
      </a>
    </div>

  </nav>
</template>