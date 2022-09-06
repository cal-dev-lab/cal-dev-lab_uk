<template>
    <div class="bg-gray-900 text-pink-500 py-5 px-6 shadow">
        <div class="md:flex mx-auto justify-between items-center max-w-5xl">
            <div class="flex items-center cursor-pointer">
                <span class="text-4xl mr-2">
                    <i class="bi bi-code"></i>
                </span>
                <h1 class="text-3xl text-white font-bold">cdl design</h1>
            </div>
            <ul class="md:flex md:items-center">
                <li v-for="item in ListItems" :key="item.id" class="md:mx-4">
                    <nuxt-link 
                        :to="item.url"
                        class="text-xl hover:text-white transition duration-300"
                    >
                        {{ item.name }}
                    </nuxt-link>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            ListItems: [
                { id: 1, url: '/', name: '/' },
                { id: 2, url: '/projects', name: '/projects' },
                { id: 3, url: '/contact', name: '/contact' }
            ]
        };
    }
}
</script>