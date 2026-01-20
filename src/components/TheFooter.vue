<script setup>
const quickLinks = [
  { id: 1, name: 'Home', href: '#home' },
  { id: 2, name: 'About Us', href: '#about' },
  { id: 3, name: 'Rooms', href: '#rooms' },
  { id: 4, name: 'Services', href: '#services' },
  { id: 5, name: 'Testimonials', href: '#testimonial' }
]

const services = [
  { id: 1, name: 'Rooms & Appartment', href: '#services' },
  { id: 2, name: 'Sports & Gaming', href: '#services' },
  { id: 3, name: 'Food & Restaurant', href: '#services' },
  { id: 4, name: 'Spa & Fitness', href: '#services' },
  { id: 5, name: 'Event & Party', href: '#services' },
  { id: 6, name: 'GYM & Yoga', href: '#services' }
]

const rooms = [
  { id: 1, name: 'Junior Suite', href: '#rooms' },
  { id: 2, name: 'Executive Suite', href: '#rooms' },
  { id: 3, name: 'Super Deluxe', href: '#rooms' }
]

const contact = [
  { id: 1, name: '+91 1234567890', href: 'tel:+911234567890' },
  { id: 2, name: 'info@juststay.com', href: 'mailto:info@juststay.com' },
  { id: 3, name: 'Ahmedabad, India', href: '#contact' },

]
</script>

<template>
  <footer id="contact" class="bg-background pt-16 pb-8">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 md:px-10">

      <div class="grid grid-cols-1 md:grid-cols-3 lg:grid-cols-5 gap-8 lg:gap-12 mb-12">
        
        <div class="lg:col-span-1 text-center md:text-left">
          <h3 class="text-heading text-2xl font-bold mb-4">
            Just<span class="text-primary">Stay</span>
          </h3>
          <p class="text-muted text-sm leading-relaxed mb-4">
            Recusandae quos nesciunt veniam eum quia 
          </p>
          <p class="text-text text-sm font-medium">
            shaikhsaad256@gmail.com
          </p>
        </div>

        <div class="lg:col-span-1 text-center md:text-left">
          <h3 class="text-heading text-lg font-bold mb-6">
            Quick Links
          </h3>
          <ul class="space-y-3">
            <li v-for="link in quickLinks" :key="link.id">
              <a 
                :href="link.href" 
                class="text-muted text-sm hover:text-primary transition-colors duration-200"
              >
                {{ link.name }}
              </a>
            </li>
          </ul>
        </div>

        <div class="lg:col-span-1 text-center md:text-left">
          <h3 class="text-heading text-lg font-bold mb-6">
            Our Services
          </h3>
          <ul class="space-y-3">
            <li v-for="service in services" :key="service.id">
              <a 
                :href="service.href" 
                class="text-muted text-sm hover:text-primary transition-colors duration-200"
              >
                {{ service.name }}
              </a>
            </li>
          </ul>
        </div>

        <div class="lg:col-span-1 text-center md:text-left">
          <h3 class="text-heading text-lg font-bold mb-6">
            Our Rooms
          </h3>
          <ul class="space-y-3">
            <li v-for="room in rooms" :key="room.id">
              <a 
                :href="room.href" 
                class="text-muted text-sm hover:text-primary transition-colors duration-200"
              >
                {{ room.name }}
              </a>
            </li>
          </ul>
        </div>

        <div class="lg:col-span-1 text-center md:text-left">
          <h3 class="text-heading text-lg font-bold mb-6">
            Contact Us
          </h3>
          <ul class="space-y-3">
            <li v-for="item in contact" :key="item.id">
              <a 
                :href="item.href" 
                class="text-muted text-sm hover:text-primary transition-colors duration-200"
              >
                {{ item.name }}
              </a>
            </li>
          </ul>
        </div>

      </div>

      <div class="border-t border-border pt-6">
        <p class="text-center text-muted text-sm">
          © 2026 JustStay. All rights reserved.
        </p>
      </div>
    </div>
  </footer>
</template>