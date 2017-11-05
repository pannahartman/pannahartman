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
    const pages = ['index', 'blog', 'shop', 'contact']

    if (pages.from && pages.to) {
      if (pages.indexOf(from.name) > pages.indexOf(to.name)) return 'slide-left'
    }

    return 'slide-right'
  }
}
</script>
