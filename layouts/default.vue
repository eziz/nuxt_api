<template>
  <div>
   
    <nuxt keep-alive :keep-alive-props="{ max: 10 }" />
    <div v-if="$nuxt.isOffline">You are offline</div>
    <Nuxt />
  </div>
</template>