<template>
<nav class="navbar">
  <div class="navbar-brand">
    <nuxt-link class="navbar-item" to="/">Panna Hartman</nuxt-link>
    <div class="navbar-burger">
      <span></span>
      <span></span>
      <span></span>
    </div>
  </div>
  <div class="navbar-menu">
    <div class="navbar-start">
      <nuxt-link class="navbar-item" to="/blog">Blog</nuxt-link>
      <nuxt-link class="navbar-item" to="/shop">Shop</nuxt-link>
      <nuxt-link class="navbar-item" to="/contact">Contact</nuxt-link>
    </div>
  </div>
</nav>
</template>

<script>
export default {
  name: 'NavBar'
}
</script>
