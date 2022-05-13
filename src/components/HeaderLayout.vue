<template>
<header>
<div class="container">
<div><img src="../assets/vue-dc-comics-1/img/dc-logo.png" alt=""></div>
<nav>
  <ul>
    <li>characters</li>
    <li>comics</li>
    <li>tv</li>
    <li>movies</li>
    <li>games</li>
    <li class="active">collectibles</li>
    <li>videos</li>
    <li>fans</li>
    <li>news</li>
    <li>shop</li>
  </ul>

</nav>
</div>
</header>
</template>

<script>
export default {
  name: "HeaderLayout"
}
</script>

<style lang="scss">
@import "../assets/style/utils";
@import "../assets/style/mixins";
@import "../assets/style/vars";
  header{
    height: 100px;
    background-color: white;
    div{
      display: flex;
      justify-content: space-between;
      nav{
        display: flex;
        align-items: center;
        li{
          @include headeNavText();
          display: inline-block;
          margin: 0 15px;
          &:hover{
            color:$principal-color;
            cursor: pointer;
          }
        }
      }

    }
  }
</style>