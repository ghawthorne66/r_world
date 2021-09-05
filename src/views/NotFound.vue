<template>
  <h1>Oops!</h1>
  <h2>The {{ resource }} you're looking for is not here</h2>
  <router-link :to="{ name: 'EventList' }">Back to the home page</router-link>

</template>

<script>
export default {
  name: 'NotFound',
  props: {
    resource: {
      type: String,
      required: true,
      default: 'page'
    }
  }
}
</script>

<style scoped>

</style>