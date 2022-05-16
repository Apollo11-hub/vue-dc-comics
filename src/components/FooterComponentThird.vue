<template>
  <section>
    <div class="container">
      <button>sing up now !</button>
      <ul>
        <li id="footer-third-title">follow us</li>
        <li><i class="fa-brands fa-facebook"></i></li>
        <li><i class="fa-brands fa-twitter"></i></li>
        <li><i class="fa-brands fa-youtube"></i></li>
        <li><i class="fa-brands fa-pinterest"></i></li>
        <li><i class="fa-solid fa-location-dot"></i></li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  name:"FooterComponentThird"
}
</script>

<style lang="scss" scoped>

@import "../assets/style/utils";
@import "../assets/style/mixins";
@import "../assets/style/vars";
  section{
    background-color:#303030;
    div{
      display: flex;
      justify-content: space-between;
      padding: 20px 0;
      button{
        padding: 20px;
        font-weight: 600;
        text-transform: uppercase;
        color: white;
        background-color: #303030;
        border: 1px solid $principal-color;
        &:hover{
          background-color: lighten($color: #303030, $amount: 10);
          cursor: pointer;
        }
        &:active{
          transform: scale(0.98);

            box-shadow: 3px 2px 22px 1px rgba(0, 0, 0, 0.24);

        
        }
      }
      ul{
        display: flex;
        li{
          @include center();
          margin-right: 20px;
          font-size: 20px;
          color: rgb(133, 132, 132);
        }
      }
    }
  }
</style>