<template>
  
  <header>
    <!-- LOGO SX ------- NAVBAR DX -->
  <div class="logo">
    <img src="../assets/img/dc-logo.png" alt="Logo">
  </div>
  
  <nav>
    <ul>
      <li>
        <a href="#">CHARACTERS</a>
      </li>
       <li>
        <a href="#">COMICS</a>
      </li>
       <li>
        <a href="#">MOVIES</a>
      </li>
       <li>
        <a href="#">TV</a>
      </li>
       <li>
        <a href="#">GAMES</a>
      </li>
       <li>
        <a href="#">VIDEOS</a>
      </li>
       <li>
        <a href="#">NEWS</a>
      </li>
       <li>
        <a href="#">SHOP</a>
      </li>      
    </ul>
  </nav>

</header>
</template>

<script>
export default {
  name: `HeaderComponent`
}
</script>

<style lang="scss" scoped>

  header{
    background-color: #fff;
    border-bottom: 1px solid #ebebeb;
    box-sizing: content-box;
    height: 115px;
    overflow: visible;
    width: 100%;
    z-index: 500;
    display: flex;
      .logo{
        left: 15px;
        line-height: 115px;
        position: absolute;
        width: 81px;
        z-index: 1;
          img{
            height: 81px;
            vertical-align: middle;
            width: 81px;
          }
        }
      nav{
        min-height: 115px;
        margin-left: auto;
        margin-right: auto;
        width: 1080px;
      }
      ul{
        display: flex;
        list-style: none;
      }
      li{
        margin-bottom: 0;
        margin-left: 20px;
        margin-right: 20px;
        margin-top: 0;
        padding-bottom: 50px;
        padding-left: 0;
        padding-top: 0;
        position: relative;
      }
      li a{
        color: #464646;
        display: block;
        padding-left: 0;
        padding-right: 0;
        text-transform: uppercase;
        font-size: 20px;
        display: inline-block;
        font-weight: bolder;
        &:hover{
          color: #0282F9;
        }
      }
  }

</style>