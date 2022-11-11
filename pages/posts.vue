<template>
    <main>
      <h1 class="green">Posts</h1>
    <NuxtLink to="/">
      Home Page
    </NuxtLink>   
  </main>
</template>
<script>
  export default {
    layout: 'blog'
    // page component definitions
  }
</script>

<script>
  export default {
    head() {
      // Set Meta Tags for this Page
    }
    // ...
  }
</script>

<style>
  .green {
    color: green;
  }
</style>