<template>
  <section id="hero" class="darktheme">
    <div class="container mx-auto">
      <header><h1>SPACE TRAVELERS</h1></header>
      <h2>We make space travel a reality<span class="cta-text">.</span><br />THAT’s it</h2>
      <h3>Yesterday Paris <span class="cta-text">-</span> London <span class="cta-text">-</span> NY <br /><span class="cta-text">Tomorrow</span> TheMoon <span class="cta-text">-</span> Mars </h3>
      <h4>Are you in <span class="cta-text">?</span></h4>
    </div>
    <div class="container mx-auto">
      <Newsletter />
    </div>
    <div class="stroke upper"></div>
    <div class="stroke lower"></div>
    <img src="@/assets/images/space-travelers-rocket.svg" alt="SpaceRocket">
  </section>
</template>

<script>
import Newsletter from '../Newsletter'
export default {
  name: 'Hero',
  components: { Newsletter }
}
</script>

<style lang="scss">
$ctaColor : #F9A826;
$darkBGColor : #121212;
#hero{
  position: relative;
  min-height: 110vh;
  color : black;
  padding-top: 10px;
  padding-bottom: 10px;
  @media screen and (min-width: 640px){
    height: 100vh;
  }
  h1{
    padding: 0 10px;
    font-weight: 700;
    font-size: 32px;
    text-transform: uppercase;
    text-align: center;
    letter-spacing: 10px;
    margin-top: 10px;
    @media (min-width: 640px) {
      font-size: 48px;
      margin-top: 30px;
      margin-bottom: 20px;
    }
  }
  h2{
    padding: 10px;
    font-weight: 700;
    font-size: 20px;
    text-transform: uppercase;
    text-align: center;
    letter-spacing: 10px;
    margin-bottom: 10px;
    @media (min-width: 640px) {
      margin-bottom: 20px;
      font-size: 26px;
    }
  }
  h3{
    padding: 0 10px;
    font-weight: 300;
    font-size: 20px;
    text-transform: uppercase;
    text-align: center;
    letter-spacing: 10px;
    margin-bottom: 10px;
    @media (min-width: 640px) {
      margin-bottom: 20px;
      font-size: 26px;
    }
  }
  h4{
    padding: 10px;
    font-weight: 300;
    font-size: 20px;
    text-align: center;
    letter-spacing: 10px;
    margin-bottom: 10px;
    @media (min-width: 640px) {
      margin-bottom: 20px;
      font-size: 26px;
    }
  }
  .cta-text{
    color: $ctaColor;
  }
  .stroke{
    display: none;
    background-color: $ctaColor;
    width: 1px;
    height: 280px;
    position: absolute;
    @media screen and (min-width: 920px){
      display: block;
    }
    &.upper{
      top: 15%;
      right: 10%;
    }
    &.lower{
      bottom: 0;
      left: 10%;
    }
  }
  img{
    z-index: 9;
    position: absolute;
    margin: auto;
    width: 240px;
    bottom: 0;
    right: 0;
    left: 0;
    @media screen and (min-width: 640px){
      width: 300px;
    }
  }
}
.darktheme{
  background-color: $darkBGColor;
  color: #fff !important;
}
</style>
