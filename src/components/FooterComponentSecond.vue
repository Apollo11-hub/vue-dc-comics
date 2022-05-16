<template>
  <section>
    <div class="container">
      <div>
        <ul>
          <li id="footer-list-title">dc comics</li>
          <li>characters</li>
          <li>comics</li>
          <li>movies</li>
          <li>tv</li>
          <li>games</li>
          <li>videos</li>
          <li>news</li>
        </ul>
        <ul>
            <li id="footer-list-title">shop</li>
            <li>shop DC</li>
            <li>shop DC collectibles</li>
        </ul>
        <ul>
          <li id="footer-list-title">DC</li>
          <li>term of use</li>
          <li>privacy policy (New)</li>
          <li>ad choices</li>
          <li>advertising</li>
          <li>jobs</li>
          <li>subscriptions</li>
          <li>talent workshops</li>
          <li>CPSC certificates</li>
          <li>ratings</li>
          <li>shops help</li>
          <li>contact us</li>
        </ul>
        <ul>
          <li id="footer-list-title">sites</li>
          <li>DC</li>
          <li>MAD</li>
          <li>DC kids</li>
          <li>DC universe</li>
          <li>Dc power visa</li>
        </ul>
      </div>
      <div>
        <img src="../assets/vue-dc-comics-1/img/dc-logo-bg.png" alt="DC-LOGO-FOOTER">
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "FooterComponentSecond"
}
</script>

<style lang="scss" scoped>
  @import "../assets/style/utils";
  @import "../assets/style/mixins";
  @import "../assets/style/vars";
    section{
      background-image: url("../assets/vue-dc-comics-1/img/footer-bg.jpg");
      div:first-child{
        display: flex;
        height: 480px;
        div:first-child{
          flex-flow: column wrap ;
          width: 50%;
          height: 100%;
          padding: 40px 0;
          color: white;
          ul{
            margin-bottom: 20px;
            li{
              margin-bottom: 10px;
              font-size: 17px;
              text-transform: capitalize;
              color:#b6b6b6 ;
              &:hover{
                color: white;
                cursor: pointer;
              }
            }
          }
        }
        div:last-child{
          @include center();
          width:50%;
          overflow: hidden;
          img{
            width: 105%;
          }
        }
      }
    }

</style>