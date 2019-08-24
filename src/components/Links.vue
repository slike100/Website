<template>
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/">Experience</router-link>
      <router-link to="/projects">Projects</router-link>
    <router-view />
    </div>
</template>

<script>
export default {
    name: 'Links'
}
</script>


<style lang="scss" scoped>

</style>