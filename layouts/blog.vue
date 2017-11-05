<template>
<transition name="layout" mode="out-in">
  <div class="container">
    <nav-bar/>

    <nuxt/>

    <foot-bar/>
  </div>
</transition>
</template>

<script>
export default {
  name: 'Blog',
  components: {
    NavBar: () => import('~/components/NavBar').then(m => m.default),
    FootBar: () => import('~/components/FootBar').then(m => m.default)
  }
}
</script>
