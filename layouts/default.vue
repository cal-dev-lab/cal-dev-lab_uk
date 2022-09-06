<template>

</template>

<script>
export default {
  // Target: https://go.nuxtjs.dev/config-target
  target: 'static',

  // Global page headers: https://go.nuxtjs.dev/config-head
  head: {
    title: 'cal-dev-lab_uk',
    htmlAttrs: {
      lang: 'en'
    },
    meta: [
      { charset: 'utf-8' },
      { name: 'viewport', content: 'width=device-width, initial-scale=1' },
      { hid: 'description', name: 'description', content: 'Front End Developer based in Cannock, Staffordshire. Visit me today to learn more about me.' },
      { name: 'format-detection', content: 'telephone=no' }
    ],
    link: [
      { rel: 'icon', type: 'image/x-icon', href: '/favicon.ico' },
      // Dynamic canonical URL
      {
        rel: "canonical",
        href: "https://cal-dev-lab.uk" + this.$route.path
      }
    ]
  },
</script>

<style>

</style>