<template>
  <div id="app">
    <HeaderComponent></HeaderComponent>
    <MainComponent>
      <GridComponent>
        <SeriesComponent v-for="serie in series" :cover="serie.thumb" :title="serie.series" :key="serie.series" />
      </GridComponent>
    </MainComponent>
    <FooterComponent></FooterComponent>
  </div>
</template>

<script>
import FooterComponent from './components/FooterComponent.vue'
import HeaderComponent from './components/HeaderComponent.vue'
import MainComponent from './components/MainComponent.vue'
import SeriesComponent from './components/SeriesComponent.vue'
import GridComponent from './components/GridComponent.vue'

import dcComics from './assets/dc-comics.json'

export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent,
    FooterComponent,
    SeriesComponent,
    GridComponent
  },
  data: () => ({
    series: dcComics,
  })
}
</script>

<style lang="scss">

@import './assets/style/general';
@import './assets/style/utilis';

#app {
  width: 100%;
}

</style>
