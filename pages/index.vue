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
    console.log(to, from)

    if (to) return 'slide-right'

    return 'slide-left'
  }
}
</script>
