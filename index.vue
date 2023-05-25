<template>
  <div v-if="provider === null">initializing...</div>
  <LoginMenu
    v-else-if="provider === 'anonymous'"
    google
    microsoft
  />
  <div v-else>
    logged in!
  </div>
</template>

<script>
  export default {
    components: {},
    data() {
      return {}
    }
  }
</script>

<style>
  body
  {
    margin: 0;
  }
</style>
