<script setup>
    const testimonials = [
        { id: 1, text: 'Nobis voluptatem magni doloribus voluptate culpa dolor est neque', name: 'Rita Conner', email: 'Sandrine.Luettgen@gmail.com'},
        { id: 2, text: 'Nobis voluptatem magni doloribus voluptate culpa dolor est neque', name: 'Woodrow McCullough', email: 'Idell.Hoppe86@yahoo.com'},
        { id: 3, text: 'Nobis voluptatem magni doloribus voluptate culpa dolor est neque', name: 'Veronica Hessel', email: 'Valentin.Homenick@gmail.com'},
        { id: 4, text: 'Nobis voluptatem magni doloribus voluptate culpa dolor est neque', name: 'George Heaney', email: 'Liliana.Howell85@hotmail.com'}
    ]
</script>

<template>
    <section id="testimonial" class=" pt-12 pb-17">
        <div class="text-center px-10 mb-12">
           <p class="text-title text-sm font-semibold tracking-wide">
            — Testimonial —
           </p> 
        </div>

        <div class="px-10 text-center mb-16">
            <h2 class="text-heading text-5xl font-bold mt-5">
                What People <span class="text-primary">Say?</span>
            </h2>
        </div>

        <div class="max-w-7xl mx-auto grid grid-cols-4 gap-6 px-4 pb-15">
            <div 
                v-for="item in testimonials"
                :key="item.id"
                class="text-center p-10"
            >

            <div class="text-primary text-6xl font-extrabold">”</div>

                <p class="text-price font-medium text-lg mb-5">
                    {{ item.text }}
                </p>

                <h3 class="text-heading font-medium text-base mb-3">
                    {{ item.name }}
                </h3>

                <p class="text-muted font-medium text-sm">
                    {{ item.email }}
                </p>
            </div>

        </div>
    </section>
</template>