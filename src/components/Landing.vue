<template>
  <div class="home">
    <section class="header">
      <h1 class="firstName">SAM</h1>
      <h2 class="secondName">Slike</h2>
    </section>
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/">Experience</router-link>
      <router-link to="/projects">Projects</router-link>
    <router-view />
    </div>
  </div>
</template>

<script>
export default {
  name: "Landing",
};
</script>


<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css?family=Unica+One&display=swap');

.home {
  display: flex;
  flex-direction: row;
  width: 100%;
  background: #FFFFFF 0% 0% no-repeat padding-box;
  opacity: 1;
  .header {
    display: flex;
    flex-direction: column;
    .firstName {
      letter-spacing: 0;
      color: #7E7E7E;
      opacity: 1;
      font-size: 99px;
      font-family: 'Unica One';
      margin: 20% 0 0 15%;
    }
    .secondName {
      text-align: left;
      font-family: 'Unica One';
      font-size: 75px;
      letter-spacing: 0;
      color: #7E7E7E;
      opacity: 1;
      margin: 0 0 0 15%;
    }
  }
  .nav {
    display: flex;
    flex-direction: column;
  }
}

</style>
