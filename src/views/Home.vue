<template>
  <div class="about">
      <div class="line"></div>
      <h2 class="aboutHeading">About Sam</h2>
      <p class="firstParagraph">Sam is a software engineer with over three years of professional experience and a demonstrated history of working in the technology industry.  With a bachelor degree in finance, Sam has a set of expertise that help him solve complex problems and approach them in a unique and efficient way.
      <br>
      <br>
      <br>
      He is passionate about web and back-end technologies. In his free time Sam enjoys playing and watching basketball, rock climbing, and climbing the nearest mountain.
      </p>
      <div class="imgContainer">
        <img :src="img" alt="" style="width: 100%">
      </div>
  </div>
</template>

<script>
import sam from '../assets/heroImg.jpg'

export default {
  name: "Home",
  data(){
    return {
      img: sam
    }
  }
};
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css?family=PT+Sans:400,700&display=swap');


.about {
    width: 100%;
    min-height: 500px;
    max-height: 2100px;
    background: #456496;
    margin: 0;
    display: grid;
    grid-template-columns: repeat(3, 33%);
    grid-template-rows: 15% 15% 70%;
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
      font-size: 37px;
      font-family: 'PT Sans', sans-serif;
      margin: 0 0 0 8%;
      grid-row: 2;
      grid-column-start: 1;
      grid-column-end: 3;
    }
    .firstParagraph {
      text-align: left;
      color: #FFFFFF;
      font-family: 'PT Sans', sans-serif;
      font-size: 20px;
      grid-column-start: 1;
      grid-column-end: 3;
      grid-row-start: 3; 
      margin: 0 13% 0 8%;
    }
    .imgContainer {
      height: 100%;
      width: 80%;
      grid-column-start: 3;
      grid-row-start: 2;
      grid-row-end: 3;
      align-items: center;
      align-self: stretch;
      justify-self: stretch;
      margin-top: 20%;
    }
    .img {
      width: 100%;
      height: 80%;

    }
}

// @media (max-width: 1000px){
//   .about {
//     grid-template-rows: 8% 15% 75%;
//   } 
// }

@media (max-width: 769px){
  .about {
    width: 100%;
    height: 1500px;
    background: #456496;
    margin: 0;
    display: grid;
    grid-template-columns: repeat(1, 100%);
    grid-template-rows: 5% 6% 20% 5% 20% 12%;
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
      font-size: 37px;
      font-family: 'PT Sans', sans-serif;
      margin: 0 0 0 8%;
      grid-row: 2;
      grid-column-start: 1;
    }
    .firstParagraph {
      text-align: left;
      color: #FFFFFF;
      font-family: 'PT Sans', sans-serif;
      font-size: 20px;
      grid-column-start: 1;
      grid-row-start: 3; 
      grid-row-end: 5;
      margin: 0 13% 0 8%;
    }
    .imgContainer {
      height: 100%;
      width: 80%;
      grid-row-start: 5;
      grid-row-end: 6;
      align-self: center;
      justify-self: center;
      align-items: center;
      grid-column-start: 1;
    }
    .img {
      width: 100%;
      height: 80%;
    }
  }
}


@media (max-width: 491px){
  .about {
    width: 100%;
    height: 1200px;
    background: #456496;
    margin: 0;
    display: grid;
    grid-template-columns: repeat(1, 100%);
    grid-template-rows: 5% 7% 25% 14% 11.5% 11.5%;
    .firstParagraph {
      grid-row-start: 3; 
      grid-row-end: 5;
    }
    .imgContainer {
      justify-self: start;      
      grid-row-start: 5;
      grid-row-end: 6;
      margin: 0 13% 0 8%;
    }
  }
}

@media (max-width: 376px){
  .about {
    width: 100%;
    height: 1100px;
    background: #456496;
    margin: 0;
    display: grid;
    grid-template-columns: repeat(1, 100%);
    grid-template-rows: 5% 7% 25% 25% 11.5% 11.5%;
    .firstParagraph {
      grid-row-start: 3; 
      grid-row-end: 5;
    }
    .imgContainer {
      justify-self: start;      
      grid-row-start: 5;
      grid-row-end: 6;
      margin: 0 13% 0 8%;

    }
  }
}
</style>
