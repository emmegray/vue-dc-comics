<template>
  <div id="sitemap">
    <div class="container">
      <div class="list" v-for="list in lists" :key="list.title">
        <h2>{{ list.title }}</h2>
        <ul>
          <li v-for="link in list.links" :key="link.url">
            <a :href="link.url">{{ link.label }}</a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: `Sitemap`,
  data: () => ({
    lists: [
      {
        title: "DC Comics",
        links: [
          { label: "Characters", url: "/#" },
          { label: "Comics", url: "/#" },
          { label: "Movies", url: "/#" },
          { label: "TV", url: "/#" },
          { label: "Games", url: "/#" },
          { label: "Videos", url: "/#" },
          { label: "News", url: "/#" },
        ],
      },

      {
        title: "Shop",
        links: [
          { label: "Shop Dc", url: "/#" },
          { label: "Shop Dc Collectibles", url: "/#" },
        ],
      },

      {
        title: "DC",
        links: [
          { label: "Terms Of Use", url: "/#" },
          { label: "Privacy Policy (New)", url: "/#" },
          { label: "Advertising", url: "/#" },
          { label: "Jobs", url: "/#" },
          { label: "Subscriptions", url: "/#" },
          { label: "CPSC Certificates", url: "/#" },
          { label: "Ratings", url: "/#" },
          { label: "Shop Help", url: "/#" },
          { label: "Contact Us", url: "/#" },
        ],
      },

      {
        title: "Sites",
        links: [
          { label: "DC", url: "/#" },
          { label: "DC UNIVERSE INFINITE", url: "/#" },
          { label: "DC Kids", url: "/#" },
          { label: "DC Shop", url: "/#" },
          { label: "MAD Magazine", url: "/#" },
        ],
      },
    ],
  }),
};
</script>

<style lang="scss" scoped>
@import "../../assets/style/vars";

#sitemap {
  background-image: url(../../assets/img/footer-bg.jpg);
  background-position: top center;
  background-repeat: no-repeat;
  background-size: cover;
  height: 400px;
  display: flex;
  .container {
    background-image: url(../../assets/img/dc-logo-bg.png);
    background-position: right center;
    background-repeat: no-repeat;
    display: flex;
    flex-wrap: wrap;
    align-content: baseline;
    flex-direction: column;
    div:nth-child(n + 3) {
      height: 100%;
    }
  }
  h2 {
    color: white;
    font-variant: small-caps;
    text-transform: lowercase;
    padding: 10px 0;
    margin-top: 20px;
    padding-right: 30px;
  }
  ul {
    padding-right: 30px;
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