<script>
export default {
  name: 'BlogLayout',
  components: {
    NavBar: () => import('~/components/NavBar').then(m => m.default || m),
    FootBar: () => import('~/components/FootBar').then(m => m.default || m)
  }
}
</script>

<template>
  <transition name="layout" mode="out-in">
    <div>
      <div class="container">
        <nav-bar/>

        <nuxt/>
      </div>

      <foot-bar/>
    </div>
  </transition>
</template>
