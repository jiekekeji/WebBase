<template>
  <div class="content">
    <div class="container">
      <router-view></router-view>
    </div>
    <!--底部的导航区域-->
    <div class="bottom-nav">
      <ul class="nav-menu">
        <li>1</li>
        <li>2</li>
        <li>3</li>
        <li>4</li>
      </ul>
    </div>
  </div>
</template>

<script>
  import store from '../store/store';

  export default{
    data(){
      return {}
    },
    components: {},
    computed: {},
    methods: {},
    created () {

    },
  }
</script>

<style scoped>
  .content {
    position: fixed;
    left: 0;
    right: 0;
    top: 0;
    bottom: 0;
    background-color: rosybrown;
  }

  .bottom-nav {
    height: 0.6rem;
    background-color: antiquewhite;
    width: 100%;
    position: fixed;
    bottom: 0;
    left: 0%;
  }

  .container {
    overflow: auto;
    position: fixed;
    left: 0;
    right: 0;
    top: 0;
    bottom: 0.6rem;
    background-color: burlywood;
  }

  .nav-menu {

  }
  .nav-menu>li{
    width: 25%;
    height: 100%;
    text-align: center;
    line-height: 0.6rem;
    float: left;
    display: inline;
    font-size: 0.2rem;
  }

</style>

