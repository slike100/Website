<template>
  <div id="app">
    <landing />   
    <router-view />
  </div>
</template>

<script>
import Landing from './components/Landing'

export default {
  components: {
    Landing,
  }
  
}
</script>

<style lang="scss" scoped>
#app {
  margin: 0;
  height: auto;
  height: 100vh;
}

</style>

