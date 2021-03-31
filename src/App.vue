<template>
  <div id="app">
    <Header />
    <Equity />
    <Securities />
    <Assets />
    <Products />
  </div>
</template>

<script>
import Header from './components/header.vue'
import Equity from './components/equity.vue'
import Securities from './components/securities.vue'
import Assets from './components/assets.vue'
import Products from './components/products.vue'

export default {
  name: 'App',
  components: {
    Header,
    Equity,
    Securities,
    Assets,
    Products
  }
}
</script>

<style lang="scss">
#app {
  font-family: "Open Sans", sans-serif;
  text-align: center;
  color: #2c3e50;
}
</style>
