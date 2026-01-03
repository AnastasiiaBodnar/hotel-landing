<script setup>
import room1Image from '../assets/room1.jpg'
import room2Image from '../assets/room2.jpg'
import room3Image from '../assets/room3.jpg'
</script>

<template>
    <section id="rooms" class="pt-10 bg-background pb-10">
        <div class="px-10 text-center mb-11">
            <p class="text-title text-sm font-semibold tracking-wide">
                — Our Rooms — 
            </p>
        </div>

        <div class="px-10 text-center mb-20">
            <h2 class="text-heading text-5xl font-bold mt-5 mb-20">
                Explore Our <span class="text-primary">Rooms</span>
            </h2>
       
        </div>

        <div class=" flex justify-center gap-7 mx-auto px-10 grid-cols-3 max-w-7xl mb-20">
            <div class="bg-white text-center">
                <img :src="room1Image" alt="Junior Suite">
                <h3 class="text-heading text-base font-medium uppercase tracking-wider mb-4 mt-8">Junior Suite</h3>
                <p class="text-price font-semibold mb-8">$150.00 / per night</p>
            </div>

             <div class="bg-white text-center">
                <img :src="room2Image" alt="Executive Suite">
                <h3 class="text-heading text-base font-medium uppercase tracking-wider mb-4 mt-8">Executive Suite</h3>
                <p class="text-price font-semibold mb-8">$250.00 / per night</p>
            </div>

             <div class="bg-white text-center">
                <img :src="room3Image" alt="Super Deluxe">
                <h3 class="text-heading text-base font-medium uppercase tracking-wider mb-2 mt-8">Super Deluxe</h3>
                <p class="text-price font-semibold mb-8">$350.00 / per night</p>
            </div>
        </div>
    </section>
</template>