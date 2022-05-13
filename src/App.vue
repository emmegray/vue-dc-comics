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

@import './assets/style/general';
@import './assets/style/utilis';
@import './assets/style/vars';

</style>
