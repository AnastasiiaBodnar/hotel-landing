<script setup>
    const links = [
        { id: 1 , name: 'Home', href: '#' },
        { id: 2 ,  name: 'About Us', href: '#about' },
        { id: 3 ,  name: 'Rooms', href: '#rooms' },
        { id: 4 ,  name: 'Services', href: '#services' }
    ]

</script>

<template>
    <footer>
        <div class="grid grid-cols-5 gap-5">

            <div class="col-span-1">
                <div>
                    Just <span class="text-primary">Stay</span>
                </div>

                <p>
                    Recusandae quos nesciunt veniam eum quia 
                </p>

                <p>
                    shaikhsaad256@gmail.com
                </p>

            </div>

            <div
                v-for="item in links"
                :key="item.id"
            >
            <h3>Quick Links</h3>
            <ul class="space-y-4">
                    <li v-for="link in links" :key="link.id">
                        <a :href="link.href" >
                            {{ link.name }}
                        </a>
                    </li>
                </ul>

            </div>

        </div>

        <div class="text-center">
             <p >
                © 2026 JustStay. All rights reserved.
            </p>
        </div>
    </footer>
</template>