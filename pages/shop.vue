<template>
  <section>
    <h2>Shop</h2>
  </section>
</template>

<script>
export default {
  name: 'Shop',
  data: () => ({
    title: 'Shop'
  }),
  head () {
    return {
      title: this.title
    }
  },
  transition (to, from) {
    if (to === 'contact') return 'slide-right'

    return 'slide-left'
  }
}
</script>
