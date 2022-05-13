<template>
  <footer>
    <Shop></Shop>
    <div id="sitemap">
      <div class="container"></div>
    </div>
    <div id="socials">
      <div class="container"></div>
    </div>
  </footer>
</template>

<script>
import Shop from "./Footer/Shop.vue";
export default {
  name: `FooterComponent`,
  components: { Shop }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/vars"

</style>