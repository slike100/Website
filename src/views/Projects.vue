<template>
  <div class="about">
    <ComingSoon />
  </div>
</template>

<script>
import ComingSoon from "../components/ComingSoon";
export default {
  name: 'Projects',
  components: {
    ComingSoon
  }
}
</script>

<style lang="scss" scoped>
  .about {
    height: 70%;
  }
</style>
