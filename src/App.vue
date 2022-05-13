<template>
  <div id="app">
    <header-component></header-component>
    <main-component></main-component>
    <footer-component></footer-component>
  </div>
</template>

<script>
import FooterComponent from './components/FooterComponent.vue'
import HeaderComponent from './components/HeaderComponent.vue'
import MainComponent from './components/MainComponent.vue'

export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent,
    FooterComponent,
  }
}
</script>

<style lang="scss">

*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: "Greta Sans Condensed Bold","Greta Sans Bold",Arial,sans-serif;
}
ul li a{
  list-style: none;
  text-decoration: none;
}
</style>
