<template>
<nav class="navbar">
  <div class="navbar-brand">
    <nuxt-link class="navbar-item" exact to="/">Panna Hartman</nuxt-link>
    <div
      class="navbar-burger"
      @click="toggleNavBar"
      :class="{ 'is-active': isActive }"
    >
      <span></span>
      <span></span>
      <span></span>
    </div>
  </div>
  <div class="navbar-menu" :class="{ 'is-active': isActive }">
    <div class="navbar-start">
      <nuxt-link class="navbar-item" exact to="/blog">Blog</nuxt-link>
      <nuxt-link class="navbar-item" to="/shop">Shop</nuxt-link>
      <nuxt-link class="navbar-item" to="/contact">Contact</nuxt-link>
    </div>
  </div>
</nav>
</template>

<script>
export default {
  name: 'NavBar',
  data: () => ({
    isActive: false
  }),
  methods: {
    toggleNavBar () {
      this.isActive = !this.isActive
    }
  }
}
</script>

<style scoped>
.navbar-burger:not(.is-active) span:nth-child(1),
.navbar-burger:not(.is-active) span:nth-child(3) {
  transform: scale(0.61803);
}
</style>
