<script>
export default {
  name: 'DefaultLayout',
  components: {
    NavBar: () => import('~/components/NavBar').then(m => m.default || m),
    FootBar: () => import('~/components/FootBar').then(m => m.default || m)
  }
}
</script>

<template>
  <transition name="layout" mode="out-in">
    <div>
      <section class="hero is-info is-bold">
        <div class="hero-head">
          <div class="container">
            <nav-bar/>
          </div>
        </div>

        <div class="hero-body">
          <div class="container has-text-centered">
            <h1 class="title">
              The new standard in &lt;insert industry here&gt;
            </h1>
            <h2 class="subtitle">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
              enim ad minim veniam, quis nostrud exercitation ullamco laboris
              nisi ut aliquip ex ea commodo consequat.
            </h2>
          </div>
        </div>
      </section>

      <section class="section">
        <div class="container">
          <nuxt/>
        </div>
      </section>

      <foot-bar/>
    </div>
  </transition>
</template>

<style scoped>
section.section {
  min-height: 50vh;
}
</style>
