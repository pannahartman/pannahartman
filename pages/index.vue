<template>
  <section>
    <h2>Panna Hartman</h2>
  </section>
</template>

<script>
export default {
  name: 'Index',
  data: () => ({
    title: 'Index'
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
