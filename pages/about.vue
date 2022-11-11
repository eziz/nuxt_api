<template>
  <main>
    <h1>About</h1>
    <NuxtLink to="/"> Home Page </NuxtLink>
    <div>
      <div>{{ content }}</div>
      <h1>I am rendered on the {{ renderedOn }} side</h1>
      <a href="tel: +(933) 63833277">+993 63833277</a>
     
      <button @click="refresh">Refresh</button>
    </div>
  </main>
</template>

<script>
export default {
  asyncData() {
    return {
      content: 'Created at: ' + new Date(),
      renderedOn: process.client ? 'client' : 'server',
    }
  },
  methods: {
    refresh() {
      this.$nuxt.refresh()
    },
  },


}
</script>