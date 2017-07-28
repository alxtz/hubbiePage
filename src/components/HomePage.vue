<template>
  <div class="root">
    <div class="container-fluid">
      <h1>Hubbie</h1>

    </div>
    <div class="background">
      <div class="imgColumn">
        <img src="~@/assets/Activity_All.png" alt="app_activities">
        <img src="~@/assets/PrizeZone.png" alt="app_activities">
        <img src="~@/assets/ActivateLoadingPage.png" alt="app_activities">
      </div>

      <div class="imgColumn">
      </div>
      <div class="imgColumn">
        <img src="~@/assets/Activity_All.png" alt="app_activities">
        <img src="~@/assets/PrizeZone.png" alt="app_activities">
        <img src="~@/assets/ActivateLoadingPage.png" alt="app_activities">
      </div>
      <div class="imgColumn">
        <img src="~@/assets/iPhonePlanet.png" alt="app_activities">
        <img src="~@/assets/iPhone7Plus.png" alt="app_activities">
        <img src="~@/assets/iPhone727.png" alt="app_activities">
        <img src="~@/assets/Bump_All.png" alt="app_activities">
      </div>
      <div class="imgColumn">
        <img src="~@/assets/Activity_All.png" alt="app_activities">
        <img src="~@/assets/PrizeZone.png" alt="app_activities">
        <img src="~@/assets/ActivateLoadingPage.png" alt="app_activities">
      </div>
      <div class="imgColumn">
        <img src="~@/assets/iPhonePlanet.png" alt="app_activities">
        <img src="~@/assets/iPhone7Plus.png" alt="app_activities">
        <img src="~@/assets/iPhone727.png" alt="app_activities">
        <img src="~@/assets/Bump_All.png" alt="app_activities">
      </div>
    </div>
  </div>
</template>

<script>

import jquery from 'jquery'
import bootstrapWebpack from 'bootstrap-webpack'

export default {
  name: 'HomePage',
  data () {
    return {
      msg: 'HomePage'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .root {
    width: 100vw;
    height: 100vh;
  }
  .container-fluid {
    height: 100vh;
    width: 100vw;
    position: absolute;
    display: none;
  }
  .background {
    // border: 2px solid red;
    height: 100vh;
    width: 100vw;
    position: absolute;
    background-color: #5e8aa7;
    display: flex;
    overflow: hidden;

    .imgColumn {
      // border: 2px solid purple;
      padding: 0;
      padding-left: 1.5vw;
      padding-right: 1.5vw;
      flex-grow: 1;
      flex-basis: 0;
      margin-left: 1vw;
      margin-right: 1vw;
      img {
        width: 100%;
        margin-bottom: 2.7vw;
        display: none;
      }
    }
    .imgColumn:first-child {
      margin-left: -6vw;
    }
    .imgColumn:last-child {
      margin-right: -6vw;
    }
    .imgColumn:nth-child(even){
      background-image: url('~@/assets/scrollBg1.png');
      background-size: 100% auto;
      animation: animatedBackground2 210s linear infinite;
    }
    .imgColumn:nth-child(odd){
      background-image: url('~@/assets/scrollBg1.png');
      background-size: 100% auto;
      animation: animatedBackground1 200s linear infinite;
    }
  }

  @-webkit-keyframes animatedBackground1 {
    from {
    	background-position:0 5000%;
    }

    to {
    	background-position:0 0;
    }
  }

  @-webkit-keyframes animatedBackground2 {
    from {
    	background-position:0 0;
    }

    to {
    	background-position:0 5000%;
    }
  }
</style>
