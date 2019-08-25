<template>
  <div class="about">
      <div class="line"></div>
      <h2 class="aboutHeading">ABOUT SAM</h2>
  </div>
</template>

<script>

export default {
  name: "Home",
  components: {
  }
};
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css?family=Unica+One&display=swap');


.about {
    height: 70%;
    min-height: 520px;
    width: 100%;
    background:linear-gradient(180deg, #959595 0%, #637F89 100%);
    margin: 0;
    display: grid;
    grid-template-columns: repeat(3, 33%);
    grid-template-rows: 15% 42.5% 42.5%;
    justify-content: space-between;	
    .line {
        border: 1px solid #FFFFFF;
        width: 95%;
        height: 0px;
        grid-column-start: 1;
        grid-column-end: 4;
        grid-row: 1;
        align-self: center;
        justify-self: center;
    }
    .aboutHeading {
      color: #FFFFFF;
      font-family: 'Unica One';
      font-size: 37px;
      margin: 0 0 0 20%;
      grid-row: 2;
      grid-column-start: 1;
      grid-column-end: 3;
    }
}
</style>
