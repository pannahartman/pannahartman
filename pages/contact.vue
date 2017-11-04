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
    if (to) return 'slide-right'

    return 'slide-left'
  }
}
</script>
