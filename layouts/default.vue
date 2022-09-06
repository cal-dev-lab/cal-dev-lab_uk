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
                    content: "Front End Developer based in Cannock, Staffordshire. Visit me today to learn more about me.",
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