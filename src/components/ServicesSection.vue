<script setup>
import roomsIcon from '../assets/rooms.png'
import sportsIcon from '../assets/sports.png'
import foodIcon from '../assets/food.png'
import spaIcon from '../assets/spa.png'
import eventIcon from '../assets/event.png'
import gymIcon from '../assets/gym.png'

const services = [
    { id: 1, icon: roomsIcon, title: 'Rooms & Appartment', description: 'Figma ipsum component variant main layer.' },
    { id: 2, icon: sportsIcon, title: 'Sports & Gaming', description: 'Figma ipsum component variant main layer.' },
    { id: 3, icon: foodIcon, title: 'Food & Restaurant', description: 'Figma ipsum component variant main layer.' },
    { id: 4, icon: spaIcon, title: 'Spa & Fitness', description: 'Figma ipsum component variant main layer.' },
    { id: 5, icon: eventIcon, title: 'Event & Party', description: 'Figma ipsum component variant main layer.' },
    { id: 6, icon: gymIcon, title: 'GYM & Yoga', description: 'Figma ipsum component variant main layer.' }    
]
</script>

<template>
    <section id="services" class="pt-12 pb-10">
        <div class="px-10 text-center mb-12">
            <p class="text-title text-sm font-semibold tracking-wide">
                — Our Services —
            </p>
        </div>

        <div class="md-10 text-center mb-16">
            <h2 class="text-heading text-5xl font-bold mt-5">
                Explore Our <span class="text-primary">Services</span>
            </h2>
        </div>

        <div class="max-w-7xl mx-auto grid grid-cols-3 gap-6 px-4">
            <div 
                v-for="service in services"
                :key="service.id"
                class="bg-white p-10 text-center transition-all duration-300 border border-border hover:bg-primary hover:text-white hover:shadow-lg group cursor-pointer"
            >
                <img :src="service.icon" :alt="service.title" class="mx-auto mb-4 h-12 w-12 group-hover:brightness-0 group-hover:invert">
                <h3 class="text-text font-bold text-lg mb-2 group-hover:text-white">
                    {{ service.title }}</h3>
                <p class="text-muted text-sm group-hover:text-white">
                    {{ service.description }}</p>
            </div>
        </div>
    </section>
</template>