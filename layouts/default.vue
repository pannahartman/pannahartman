<template>
<transition name="layout" mode="out-in">
  <div>
    <section class="hero is-info is-bold">
      <div class="hero-head">
        <div class="container">
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
                <nuxt-link class="navbar-item" to="contact">Contact</nuxt-link>
              </div>
            </div>
          </nav>
        </div>
      </div>
      <div class="hero-body">
        <div class="container has-text-centered">
          <h1 class="title">
            The new standard in &lt;insert industry here&gt;
          </h1>
          <h2 class="subtitle">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
          </h2>
        </div>
      </div>
    </section>

    <section class="section">
      <div class="container">
        <nuxt/>
      </div>
    </section>

    <footer class="footer">
      <div class="container">
        <div class="content has-text-centered">
          <p>
            &copy; Panna Hartman 2017
          </p>
        </div>
      </div>
    </footer>
  </div>
</transition>
</template>

<script>
export default {
  name: 'Default'
}
</script>

<style scoped>
section.section {
  min-height: 60vh;
}
</style>
