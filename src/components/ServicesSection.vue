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
    <section id="services" class="pt-8">
        <div>
            <p>
                — Our Services —
            </p>
        </div>

        <div>
            <h2>
                Explore Our <span>Services</span>
            </h2>
        </div>

        <div>
            <div 
                v-for="service in services"
                :key="service.id"
            >
                <img :src="service.icon" :alt="service.title">
                <h3>{{ service.title }}</h3>
                <p>{{ service.description }}</p>
            </div>
        </div>
    </section>
</template>