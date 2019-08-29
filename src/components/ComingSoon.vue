<template>
    <div class="comingSoon">
        <h3 class="heading">Coming Soon! In the meantime checkout out my Github profile here: <a href="https://github.com/slike100" class="github">Slike100</a></h3>
    </div>
</template>

<script>
export default {
    name: 'ComingSoon'
}
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css?family=Unica+One&display=swap');

.comingSoon {
    width: 100%;
    height: 100%;
    background: #456496;
    .heading {
      font-family: 'Unica One';
      color: white;
      padding-top: 12%;
      text-align: center;
      .github {
        text-decoration: none;
        color: white;
          &:hover {
              text-decoration: underline;
          }
          &:active {
              text-decoration: none;
              color: white;
          }
      }
    }
}
</style>