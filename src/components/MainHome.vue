<template>
  <div class="content" id="main-home">
    <div class="title">首页</div>
    <div class="swiper-container">
      <div class="swiper-wrapper">
        <div class="swiper-slide">Slide 1</div>
        <div class="swiper-slide">Slide 2</div>
        <div class="swiper-slide">Slide 3</div>
      </div>
      <!--1、指示点放在这或放在外面-->
      <div class="swiper-pagination"></div>
    </div>
  </div>
</template>
<style scoped>
  @import "../assets/swiper/swiper-3.4.0.min.css";
  @import "../assets/dialog/jk-widget-sty.css";

  .title {
    text-align: center;
    line-height: 0.4rem;
    font-size: 0.2rem;
    height: 0.4rem;
    width: 100%;
    background-color: aliceblue;
  }

  .swiper-container {
    width: 100%;
    height: 1.4rem;
    background-color: antiquewhite;
    font-size: 0.2rem;
  }
</style>
<script>
  import Swiper from '../assets/swiper/swiper-3.4.0.jquery.min'
  require('../assets/dialog/jk-dialog');
  export default{
    data(){
      return {
        msg: 'hello vue'
      }
    },
    components: {},
    mounted: function () {
      var mySwiper = new Swiper('.swiper-container', {
        pagination: '.swiper-pagination',
        paginationClickable: true
      });
//      jkDialog.showToastOverlay('1230');
    }
  }
</script>
