<template>
  <div class="home">
    <h1>Home</h1>
    <button @click='logout'>Logout</button>
  </div>
</template>

<script>
export default {
  name: 'Home',
  methods: {
    logout() {
      this.$store.commit('changeAuth')
      this.$router.push('/login')
    }
  }
}
</script>