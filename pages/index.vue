<template>
  <main>
    <h1>Home page</h1>
    <NuxtLink to="/about">
      About (internal link that belongs to the Nuxt App)
    </NuxtLink>
    <br />
    <NuxtLink to="/contact"> Contact </NuxtLink>
    <br />
    <NuxtLink to="/posts"> Posts </NuxtLink>
    <MountainsList />
    <br />
    <a href="https://nuxtjs.org">NuxtJs web site</a>
    <br />
    <a href="https://bildirisyeri.com">Bildirisyeri</a>
  </main>
</template>

<script>
export default {
  name: 'IndexPage',

  beforeMount() {
    // window.alert('Start')
  },
  mounted() {
    this.$nextTick(() => {
      this.$nuxt.$loading.start()
      setTimeout(() => this.$nuxt.$loading.finish(), 500)
    })
   // window.alert('finish')
  },
 
}
</script>
