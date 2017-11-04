<template>
  <section>
    <h2>Blog</h2>
  </section>
</template>

<script>
export default {
  name: 'Blog',
  data: () => ({
    title: 'Blog'
  }),
  head () {
    return {
      title: this.title
    }
  }
}
</script>
