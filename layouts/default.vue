<template>
  <div class="root">
    <Nuxt />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: 'HypeATX',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'A company dedicated to the culture.'
        }
      ]
    }
  }
}
</script>

<style>
</style>
