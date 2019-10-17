<template>
  <div id="app">
    <h1>Dosi - Reconstrucao</h1>
    <HomePage />
  </div>
</template>

<script>
const Home = () => import('./pages/Home')

export default {
  components: {
    HomePage: Home
  }
}
</script>
