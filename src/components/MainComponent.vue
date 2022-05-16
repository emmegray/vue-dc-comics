<template>
  <main>
      <img src="../assets/img/jumbotron.jpg" alt="Jumbotron" />
      <div class="container">
        <div class="jumbotron">
          <slot></slot>
        </div>
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
      
  img {
    overflow: hidden;
    width: 100%;
    height: auto;
  }

  .container {
    margin: 0 auto;
    
    .jumbotron {
      padding: 20px 0;
      position: relative;
      display: block;
    }
  }
}

</style>