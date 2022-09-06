<template>
    <div>
        <Navbar />
        <nuxt />
    </div>
</template>

<script>
import Navbar from '~/components/Navbar.vue'

export default {
    head() {
        return {
            meta: [
                {
                    hid: "description",
                    name: "description",
                    content: "Best place for dad jokes.",
                }
            ],
            link: [
                // Dynamic canonical URL
                {
                    rel: "canonical",
                    href: "https://cal-dev-lab.uk" + this.$route.path
                },
                // Bootstrap icons
                {
                    rel: "stylesheet",
                    href: "https://cdn.jsdelivr.net/npm/bootstrap-icons@1.9.1/font/bootstrap-icons.css"
                }
            ],
        }
    },
    components: { Navbar }
}
</script>