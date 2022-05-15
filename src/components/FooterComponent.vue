<template>
  <footer>
    <Shop></Shop>
    <Sitemap></Sitemap>
    <Socials></Socials>
  </footer>
</template>

<script>
import Shop from "./Footer/Shop.vue";
import Sitemap from "./Footer/Sitemap.vue";
import Socials from "./Footer/Socials.vue";
export default {
  name: `FooterComponent`,
  components: { Shop, Sitemap, Socials }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/vars";

footer {
  position: fixed;
  left: 0;
  bottom: 0;
  width: 100%;
}
</style>