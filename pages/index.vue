<template>
  <div>
    loading
  </div>
</template>

<script>

export default {
  layout: 'menu',
  mounted () {
    this.$router.push({name: `list`})
  }
}
</script>
