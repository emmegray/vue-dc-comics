<template>
  <div class="series">
    <img :src="`${cover}`"/>
    <h4 class="title">{{title}}</h4>
  </div>
</template>

<script>
export default {
  name: "SeriesComponent",
  props: {
    cover: String,
    title: String,
  }
}
</script>

<style lang="scss" scoped>

  .series {
    img {
      width: 100%;
      margin-bottom: 10px;
    }
    .title {
      text-transform: uppercase;
      font-variant: small-caps;
      color: lightgrey;
    }
  }
</style>