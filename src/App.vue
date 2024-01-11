<template>
  <div>
    <router-link :to="{ name: 'home' }">Home</router-link> |
    <router-link :to="{ name: 'about' }">About</router-link> |
    <router-link :to="{ name: 'Counter' }">Counter</router-link>
  </div>
  <router-view></router-view>
</template>

<script>

</script>