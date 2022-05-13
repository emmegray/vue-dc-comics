<template>
  <div id="sitemap">
    <div class="container">
      <ul>
        <h2>dc comics</h2>
        <li v-for="dcComics in dcComics" :key="dcComics.url">
          <a :href="dcComics.url">{{dcComics.label}}</a>
        </li>
        <h2>shop</h2>
        <li v-for="dcShop in dcShop" :key="dcShop.url">
          <a :href="dcShop.url">{{dcShop.label}}</a>
        </li>
        <h2>dc</h2>
        <li v-for="dC in dC" :key="dC.url">
          <a :href="dC.url">{{dC.label}}</a>
        </li>
            <h2>sites</h2>
        <li v-for="sites in sites" :key="sites.url">
          <a :href="sites.url">{{sites.label}}</a>
        </li>
      </ul>
      <!-- <img src="../../assets/img/dc-logo-bg.png"/> -->
    </div>
  </div>
</template>

<script>
export default {
name: `Sitemap`,
data:() => ({
  dcComics: [
    {label: "Characters", url: "/#"},
    {label: "Comics", url: "/#"},
    {label: "Movies", url: "/#"},
    {label: "TV", url: "/#"},
    {label: "Games", url: "/#"},
    {label: "Videos", url: "/#"},
    {label: "News", url: "/#"},
    ],

  dcShop: [
    {label: "Shop Dc", url: "/#"},
    {label: "Shop Dc Collectibles", url: "/#"},
  ],

    dC: [
    {label: "Terms Of Use", url: "/#"},
    {label: "Privacy Policy (New)", url: "/#"},
    {label: "Advertising", url: "/#"},
    {label: "Jobs", url: "/#"},
    {label: "Subscriptions", url: "/#"},
    {label: "CPSC Certificates", url: "/#"},
    {label: "Ratings", url: "/#"},
    {label: "Shop Help", url: "/#"},
    {label: "Contact Us", url: "/#"},
  ],

    sites: [
    {label: "DC", url: "/#"},
    {label: "DC UNIVERSE INFINITE", url: "/#"},
    {label: "DC Kids", url: "/#"},
    {label: "DC Shop", url: "/#"},
    {label: "MAD Magazine", url: "/#"},
  ]
})
};
</script>

<style lang="scss" scoped>
@import "../../assets/style/vars";

#sitemap {
  background-image: url(../../assets/img/footer-bg.jpg);
  height: 400px;
  padding: 20px 0;
  h2 {
  color: white;
  font-variant: small-caps;
  padding: 10px 0;
  }
  a {
    font-size: small;
    color: #696969;
    &:hover {
    color: lightgrey;
    }
  }
}
</style>