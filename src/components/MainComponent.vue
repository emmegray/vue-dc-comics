<template>
  <main>
      <img src="../assets/img/jumbotron.jpg" alt="Jumbotron" />
      <div class="container">
        <div class="jumbotron">
          <h2>Current series</h2>
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
    height: ato;
  }

  .container {
    margin: 0 auto;
    
    .jumbotron {
      padding: 40px 0 20px 0;
      position: relative;
      display: block;

      h2{
        position: absolute;
        top: -30px;
        background: $primary-color;
        padding: 10px 20px;
        text-transform: uppercase;
      }
    }
  }
}

</style>