<script setup>
import { ref, onMounted } from 'vue'
import bgImage from '../assets/background.png'

const isLoaded = ref(false)
const showBookingModal = ref(false)
const showVideoModal = ref(false)

onMounted(() => {
  setTimeout(() => {
    isLoaded.value = true
  }, 100)
})

const openBooking = () => {
  showBookingModal.value = true
}

const closeBooking = () => {
  showBookingModal.value = false
}

const openVideo = () => {
  showVideoModal.value = true
}

const closeVideo = () => {
  showVideoModal.value = false
}

const handleBooking = (event) => {
  event.preventDefault()
  alert('Your reservation has been sent! We will contact you shortly.')
  closeBooking()
}
</script>

<template>
  <section id="home" class="relative h-screen w-full flex items-end justify-start text-left px-4 sm:px-8 md:px-10 lg:px-14 xl:px-20 pb-12">
    
    <div 
      class="absolute inset-0 bg-cover bg-center"
      :style="{ backgroundImage: `url(${bgImage})` }"
    ></div>

    <div class="absolute inset-0 bg-linear-to-r from-black/70 via-black/50 to-transparent"></div>

    <div class="relative z-10 text-white max-w-full sm:max-w-xl md:max-w-2xl lg:max-w-3xl xl:max-w-4xl">
      <p class="text-base sm:text-lg md:text-xl font-semibold leading-relaxed mb-2 text-white/90">
        Welcome to
      </p>
      
      <h1 class="text-3xl sm:text-4xl md:text-5xl lg:text-5xl xl:text-6xl font-bold leading-snug mb-4 sm:mb-5 md:mb-6">
        Hotel Just<span class="text-primary">Stay</span>
      </h1>
      
      <h2 class="text-3xl sm:text-4xl md:text-5xl lg:text-5xl xl:text-6xl font-bold mb-6 sm:mb-7 md:mb-8">
        Ahmedabad, India
      </h2>
      
      <p class="text-gray-200 text-sm sm:text-base md:text-lg lg:text-xl leading-relaxed mb-8 sm:mb-9 md:mb-10 max-w-xl lg:max-w-2xl">
        Experience luxury and comfort in the heart of Ahmedabad. 
        From elegant rooms to world-class amenities, we make every stay unforgettable.
      </p>
      
      <div class="flex flex-col sm:flex-row gap-4 sm:gap-5 justify-start">
        <button class="bg-primary hover:bg-orange-600 text-white px-8 sm:px-10 py-3 rounded-2xl font-bold text-base sm:text-lg transition transform cursor-pointer">
          Book Now
        </button>
        
        <button 
          @click="openVideo"
          class="group relative border-2 border-white text-white hover:bg-white hover:text-gray-900 px-8 sm:px-10 py-3 sm:py-4 rounded-2xl font-bold text-base sm:text-lg transition-all duration-300 transform hover:scale-105 hover:shadow-2xl cursor-pointer overflow-hidden"
        >
          <span class="relative z-10 flex items-center justify-center gap-2">
            Watch Video
          </span>
          <span class="absolute inset-0 bg-white transform scale-x-0 group-hover:scale-x-100 transition-transform duration-300 origin-left"></span>
        </button>
      </div>
    </div>

    <div 
      v-if="showBookingModal"
      class="fixed inset-0 bg-black/60 backdrop-blur-sm flex items-center justify-center z-50 px-4"
      @click.self="closeBooking"
    >
      <div class="bg-white rounded-3xl p-6 sm:p-8 max-w-md w-full transform transition-all duration-300 scale-100">
        <div class="flex justify-between items-center mb-6">
          <h3 class="text-2xl sm:text-3xl font-bold text-gray-900">Book Your Stay</h3>
          <button 
            @click="closeBooking"
            class="text-gray-400 hover:text-gray-600 transition-colors"
          >
            <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
            </svg>
          </button>
        </div>
        
        <form @submit="handleBooking" class="space-y-4">
          <div>
            <label class="block text-sm font-semibold text-gray-700 mb-2">Full Name</label>
            <input 
              type="text" 
              required
              class="w-full px-4 py-3 border-2 border-gray-200 rounded-xl focus:border-primary focus:outline-none transition-colors"
              placeholder="John Doe"
            />
          </div>
          
          <div>
            <label class="block text-sm font-semibold text-gray-700 mb-2">Email</label>
            <input 
              type="email" 
              required
              class="w-full px-4 py-3 border-2 border-gray-200 rounded-xl focus:border-primary focus:outline-none transition-colors"
              placeholder="john@example.com"
            />
          </div>
          
          <div>
            <label class="block text-sm font-semibold text-gray-700 mb-2">Phone</label>
            <input 
              type="tel" 
              required
              class="w-full px-4 py-3 border-2 border-gray-200 rounded-xl focus:border-primary focus:outline-none transition-colors"
              placeholder="+91 12345 67890"
            />
          </div>
          
          <div class="grid grid-cols-2 gap-4">
            <div>
              <label class="block text-sm font-semibold text-gray-700 mb-2">Check-in</label>
              <input 
                type="date" 
                required
                class="w-full px-4 py-3 border-2 border-gray-200 rounded-xl focus:border-primary focus:outline-none transition-colors"
              />
            </div>
            <div>
              <label class="block text-sm font-semibold text-gray-700 mb-2">Check-out</label>
              <input 
                type="date" 
                required
                class="w-full px-4 py-3 border-2 border-gray-200 rounded-xl focus:border-primary focus:outline-none transition-colors"
              />
            </div>
          </div>
          
          <div>
            <label class="block text-sm font-semibold text-gray-700 mb-2">Room Type</label>
            <select 
              required
              class="w-full px-4 py-3 border-2 border-gray-200 rounded-xl focus:border-primary focus:outline-none transition-colors"
            >
              <option value="">Select a room</option>
              <option value="junior">Junior Suite - $150/night</option>
              <option value="executive">Executive Suite - $250/night</option>
              <option value="super">Super Deluxe - $350/night</option>
            </select>
          </div>
          
          <div>
            <label class="block text-sm font-semibold text-gray-700 mb-2">Guests</label>
            <select 
              required
              class="w-full px-4 py-3 border-2 border-gray-200 rounded-xl focus:border-primary focus:outline-none transition-colors"
            >
              <option>1 Guest</option>
              <option>2 Guests</option>
              <option>3 Guests</option>
              <option>4+ Guests</option>
            </select>
          </div>
          
          <button 
            type="submit"
            class="w-full bg-primary hover:bg-orange-600 text-white py-4 rounded-xl font-bold text-lg transition-all duration-300 transform hover:scale-105 hover:shadow-xl mt-6"
          >
            Confirm Booking
          </button>
        </form>
      </div>
    </div>

    <div 
      v-if="showVideoModal"
      class="fixed inset-0 bg-black/80 backdrop-blur-sm flex items-center justify-center z-50 px-4"
      @click.self="closeVideo"
    >
      <div class="relative max-w-4xl w-full">
        <button 
          @click="closeVideo"
          class="absolute -top-12 right-0 text-white hover:text-primary transition-colors"
        >
          <svg class="w-8 h-8" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
          </svg>
        </button>
        
        <div class="bg-black rounded-2xl overflow-hidden aspect-video">
          <iframe 
            class="w-full h-full"
            src="https://www.youtube.com/embed/Bo_CQWw6XtQ?autoplay=1" 
            title="Hotel Tour Video"
            frameborder="0" 
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
            allowfullscreen
          ></iframe>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
@keyframes bounce-slow {
  0%, 100% { 
    transform: translateY(0); 
  }
  50% { 
    transform: translateY(-10px); 
  }
}

.animate-bounce-slow {
  animation: bounce-slow 3s ease-in-out infinite;
}
</style>