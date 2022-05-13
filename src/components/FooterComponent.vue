<template>
  <footer>
    <Shop></Shop>
    <Sitemap></Sitemap>
    <div id="socials">
      <div class="container"></div>
    </div>
  </footer>
</template>

<script>
import Shop from "./Footer/Shop.vue";
import Sitemap from "./Footer/Sitemap.vue";
export default {
  name: `FooterComponent`,
  components: { Shop, Sitemap }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/vars"

</style>