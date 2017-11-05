<script>
export default {
  name: 'FootBar',
  data: () => ({
    currentYear: new Date().getFullYear()
  })
}
</script>

<template>
  <footer class="footer">
    <div class="container">
      <div class="content has-text-centered">
        <p>&copy; Panna Hartman {{ currentYear }}</p>
      </div>
    </div>
  </footer>
</template>
