<template>
  <main>
    <div class="container">
      <slot></slot>
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
  .container {
    margin: 0 auto;
  }
}

</style>