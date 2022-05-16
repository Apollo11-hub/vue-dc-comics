<template>
  <section>
    <div class="image-container">
        <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY" alt="comic.series">
    </div>
    <p>Action</p> 

  </section>

</template>

<script>
export default {
  name:"MainComponentCard",
  props:{
    comic:Object,
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/utils";
@import "../assets/style/mixins";
@import "../assets/style/vars";
  section{
    display: flex;
    flex-wrap:wrap ;
    div{
      width: 200px;
      height: 250px;
      margin:20px 20px 30px 0;
      .image-container{
        height: 80%;
        overflow: hidden;
        img{
          width: 100%;
        }
      }
      p{
        display: flex;
        align-items: center;
        height: 20%;
        font-size: 18px;
        text-transform:uppercase;
        color: white;
      }
    }
  }
</style>