<script setup>
import aboutImage from '../assets/about.png'
</script>

<template>
    <section id="rooms" class="pt-5 bg-background" >
        <div>
            <p>
                — Our Rooms — 
            </p>

            <h2>
                Explore Our Rooms
            </h2>
        </div>

        <div>
            <div>
                <img :src="aboutImage" alt="Junior Suite">
                <h3>Junior Suite</h3>
                <p>$150.00 / per night</p>
            </div>

             <div>
                <img :src="aboutImage" alt="Executive Suite">
                <h3>Executive Suite</h3>
                <p>$250.00 / per night</p>
            </div>

             <div>
                <img :src="aboutImage" alt="Super Deluxe">
                <h3>Super Deluxe</h3>
                <p>$350.00 / per night</p>
            </div>
        </div>
    </section>
</template>