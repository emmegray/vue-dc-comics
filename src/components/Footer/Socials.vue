<template>
  <div id="social">
    <div class="container">
      <a href="#"><button class="btn">SING-UP NOW!</button></a>
      <div class="social-icons">
        <h2>Follow us</h2>
        <li v-for="socialIcons in socialIcons" :key="socialIcons.label">
          <a :href="socialIcons.url">
            <img :src="`/img/${socialIcons.src}`"/>
            </a>
        </li>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: `Social`,
  data:() => ({
    socialIcons: [
      {label: "facebook", url: "/#", src:"footer-facebook.png"},
      {label: "twitter", url: "/#", src:"footer-twitter.png"},
      {label: "youtube", url: "/#", src:"footer-youtube.png"},
      {label: "pinterest", url: "/#", src:"footer-pinterest.png"},
      {label: "periscope", url: "/#", src:"footer-periscope.png"},
    ]
  })
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/vars";

#social {
  background-color: $bg-gray;
  text-transform: uppercase;
  padding: 20px;
  .container {
  display: flex;
  flex-wrap: wrap;
  box-sizing: border-box;
  }
  button {
  background-color: transparent;
  color: white;
  justify-self: flex-start;
  &:hover{
    background: #0282F9;
  }
  }
  .social-icons {
  display: flex;
  }
  h2 {
  color: $primary-color;
  }
}


</style>