<script setup>
import roomsIcon from '../assets/rooms.png'
import sportsIcon from '../assets/sports.png'
import foodIcon from '../assets/food.png'
import spaIcon from '../assets/spa.png'
import eventIcon from '../assets/event.png'
import gymIcon from '../assets/gym.png'
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
                Explore Our <span class="text-primary">Services</span>
            </h2>
        </div>

        <div>
            <div>
                <img :src="roomsIcon" alt="Rooms Icon">
                <h3>Rooms & Appartment</h3>
                <p>Figma ipsum component variant main layer.</p>
            </div>

            <div>
                <img :src="sportsIcon" alt="Sports Icon">
                <h3>Sports & Gaming</h3>
                <p>Figma ipsum component variant main layer.</p>
            </div>

            <div>
                <img :src="foodIcon" alt="Food Icon">
                <h3>Food & Restaurant</h3>
                <p>Figma ipsum component variant main layer.</p>
            </div>

            <div>
                <img :src="spaIcon" alt="Spa Icon">
                <h3>Spa & Fitness</h3>
                <p>Figma ipsum component variant main layer.</p>
            </div>

            <div>
                <img :src="eventIcon" alt="Event Icon">
                <h3>Event & Party</h3>
                <p>Figma ipsum component variant main layer.</p>
            </div>

            <div>
                <img :src="gymIcon" alt="Gym Icon">
                <h3>GYM & Yoga</h3>
                <p>Figma ipsum component variant main layer.</p>
            </div>
        </div>
    </section>
</template>