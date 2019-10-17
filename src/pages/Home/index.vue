<template>
  <transition name="fade" apper>
    <div @click="classActive = !classActive" :class="{active: classActive}">
      <h1>{{ title }}</h1>
    </div>
  </transition>
</template>

<script>
export default {

  data () {
    return {
      title: 'Home Page',
      classActive: true
    }
  },
  methods: {
    tabClick () {
      alert('Teste')
    }
  }

}
</script>

<style lang="scss" scoped>
  @import url('https://fonts.googleapis.com/css?family=Roboto:300,400,500,700&display=swap');

  div {
    background:#333;
    user-select: none;
    border-radius:8px;
    box-sizing: border-box;
    padding:16px;

    h1{
      margin:0;
      padding:0;
      font-family:'Roboto';
      color:#EEE;
    }
  }

  .active{
    background:#229933;
  }

  // Animation tag to transition Vue
  .fade-enter-active {
    transition: all .3s ease;
  }
  .fade-leave-active {
    transition: all .8s cubic-bezier(1.0, 0.5, 0.8, 1.0);
  }
  .fade-enter, .fade-leave-to{
    transform: translateX(10px);
    opacity: 0;
  }
</style>
