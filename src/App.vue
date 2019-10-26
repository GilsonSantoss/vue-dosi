<template>
  <div id="app">
    <router-view></router-view>
  </div>
</template>

<style lang='scss'>
  *{
    margin:0;
    padding:0;
    box-sinzing:border-box;
    &::after,&::before{
      box-sinzing:border-box;
    }
  }
  html,body{
    width:100%;
    height:100%;
    margin:0;
    padding:0;
    position:relative;
    background-color: #e9edf0;
  }
  p, hr, ul {
    margin: 0;
    padding: 0;
  }
</style>
