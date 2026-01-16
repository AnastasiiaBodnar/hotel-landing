<script setup>
    const testimonials = [
        { id: 1, text: 'Nobis voluptatem magni doloribus voluptate culpa dolor est neque', name: 'Rita Conner', email: 'Sandrine.Luettgen@gmail.com'},
        { id: 2, text: 'Nobis voluptatem magni doloribus voluptate culpa dolor est neque', name: 'Woodrow McCullough', email: 'Idell.Hoppe86@yahoo.com'},
        { id: 3, text: 'Nobis voluptatem magni doloribus voluptate culpa dolor est neque', name: 'Veronica Hessel', email: 'Valentin.Homenick@gmail.com'},
        { id: 4, text: 'Nobis voluptatem magni doloribus voluptate culpa dolor est neque', name: 'George Heaney', email: 'Liliana.Howell85@hotmail.com'}
    ]
</script>

<template>
    <section>
        <div>
           <p>
            — Testimonial —
           </p> 
        </div>

        <div>
            <h2>
                What People Say?
            </h2>
        </div>

        <div class="grid grid-cols-4 gap-6">

            <div 
                v-for="item in testimonials"
                :key="item.id"
                class="text-center"
            >

            <div>”</div>
                <p>
                    {{ item.text }}
                </p>

                <h3>
                    {{ item.name }}
                </h3>

                <p>
                    {{ item.email }}
                </p>
            </div>

        </div>
    </section>
</template>