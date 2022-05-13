<template>
  <main>
    <div class="container">
      <slot></slot>
      <!-- <div class="jumbotron">
        <img src="../assets/img/jumbotron.jpg" alt="Jumbotron">
      </div> -->
    </div>
  </main>
</template>

<script>
export default {
  name: `MainComponent`
}
</script>

<style lang="scss" scoped>
@import "../assets/style/vars";

main {
  color: white;
  background-color: $bg-dark;
  padding: 50px 0;
  display: flex;
  .container {
    margin: 0 auto;
    .jumbotron {
      position: relative;
        display: block;
      
      img {
        overflow: hidden;
        max-width: 100%;
        height: auto;
      }
    }
  }
}

</style>