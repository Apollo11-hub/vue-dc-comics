<template>

  <nav>
    <ul class="container">
      <li>
        <img src="../assets/vue-dc-comics-1/img/buy-comics-digital-comics.png" alt="">
        <span>digital comics</span>
      </li>
      <li>
        <img src="../assets/vue-dc-comics-1/img/buy-comics-merchandise.png" alt="">
        <span>digital comics</span>
      </li>
      <li>
        <img src="../assets/vue-dc-comics-1/img/buy-comics-shop-locator.png" alt="">
        <span>digital comics</span>
      </li>
      <li>
        <img src="../assets/vue-dc-comics-1/img/buy-comics-subscriptions.png" alt="">
        <span>digital comics</span>
      </li>
      <li>
        <img src="../assets/vue-dc-comics-1/img/buy-dc-power-visa.svg" alt="">
        <span>digital comics</span>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: "FooterComponentFirst"
}
</script>

<style lang="scss" scoped>
@import "../assets/style/utils";
@import "../assets/style/mixins";
@import "../assets/style/vars";
  nav{
    @include center();
    background-color: $principal-color;
    padding: 60px 0;
    ul{
      display: flex;
      justify-content: space-around;
      width: 100%;
      li{
        @include center();
        img{
          width: 50px;
        }
        span{
          margin-left: 20px;
          font-size: 17px;
          text-transform: uppercase;
          color: white;
        }
      }
    }
  }
</style>