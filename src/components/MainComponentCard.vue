<template>
  <section>
    <div class="image-container">
        <img :src="comic.thumb" :alt="comic.series">
    </div>
    <p>{{comic.series}}</p> 

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
    div{
      width: 200px;
      margin:20px 20px 30px 0;
      .image-container{
        height: 60%;
        overflow: hidden;
        img{
          width: 100%;
        }
      }
      p{
        display: flex;
        align-items: center;
        width: 200px;

        text-transform:uppercase;
        color: white;
      }
    }

</style>