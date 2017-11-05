<template>
  <section>
    <h2>Contact</h2>
  </section>
</template>

<script>
export default {
  name: 'Contact',
  data: () => ({
    title: 'Contact'
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
