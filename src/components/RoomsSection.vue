<script setup>
import room1Image from '../assets/room1.jpg'
import room2Image from '../assets/room2.jpg'
import room3Image from '../assets/room3.jpg'
</script>

<template>
    <section id="rooms" class="pt-8 md:pt-10 xl:pt-12 bg-background  pb-8 md:pb-10 xl:pb-5">
        <div class="px-5 md:px-10 text-center mb-6 md:mb-8 lg:mb-11">
            <p class="text-title text-xs md:text-sm font-semibold tracking-wide">
                — Our Rooms — 
            </p>
        </div>

        <div class="px-5 md:px-10 text-center mb-8 md:mb-10 lg:mb-20">
            <h2 class="text-heading text-3xl md:text-4xl lg:text-5xl font-bold mt-3 md:mt-5">
                Explore Our <span class="text-primary">Rooms</span>
            </h2>
        </div>

        <div class="flex flex-col lg:flex-row justify-center gap-4 md:gap-5 lg:gap-7 mx-auto px-5 md:px-10 max-w-7xl mb-8 lg:mb-20">
            <div class="bg-white text-center w-full lg:w-1/3">
                <img :src="room1Image" alt="Junior Suite" class="w-full h-auto">
                <h3 class="text-heading text-sm md:text-base font-medium uppercase tracking-wider mb-3 md:mb-4 mt-6 md:mt-8">Junior Suite</h3>
                <p class="text-price font-semibold mb-6 md:mb-8 text-sm md:text-base">$150.00 / per night</p>
            </div>

            <div class="bg-white text-center w-full lg:w-1/3">
                <img :src="room2Image" alt="Executive Suite" class="w-full h-auto">
                <h3 class="text-heading text-sm md:text-base font-medium uppercase tracking-wider mb-3 md:mb-4 mt-6 md:mt-8">Executive Suite</h3>
                <p class="text-price font-semibold mb-6 md:mb-8 text-sm md:text-base">$250.00 / per night</p>
            </div>

            <div class="bg-white text-center w-full lg:w-1/3">
                <img :src="room3Image" alt="Super Deluxe" class="w-full h-auto">
                <h3 class="text-heading text-sm md:text-base font-medium uppercase tracking-wider mb-3 md:mb-4 mt-6 md:mt-8">Super Deluxe</h3>
                <p class="text-price font-semibold mb-6 md:mb-8 text-sm md:text-base">$350.00 / per night</p>
            </div>
        </div>
    </section>
</template>