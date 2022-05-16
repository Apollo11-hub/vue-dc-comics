<template>
<header>
<div class="container">
<div><img src="../assets/vue-dc-comics-1/img/dc-logo.png" alt=""></div>
<nav>
  <ul>

    <li v-for="(item, index) in menuItems" :key="index"
    >
      <a :class="{'activeItem': item.isClicked}" href=""> {{item.title}}</a>
      <div :class="{'activeBar' : item.isClicked}"></div>
    </li>
  </ul>

</nav>
</div>
</header>
</template>

<script>
export default {
  name: "HeaderLayout",

  data() {
    return {
      menuItems:[
        {
          title:"characters",
          linkTo:"#",
          isClicked:true
        },
        {
          title:"comics",
          linkTo:"#",
          isClicked:false
        },
        {
          title:"tv",
          linkTo:"#",
          isClicked:false
        },
        {
          title:"movies",
          linkTo:"#",
          isClicked:false
        },
        {
          title:"games",
          linkTo:"#",
          isClicked:false
        },
        {
          title:"collectibles",
          linkTo:"#",
          isClicked:false
        },
        {
          title:"videos",
          linkTo:"#",
          isClicked:false
        },
        {
          title:"fans",
          linkTo:"#",
          isClicked:false
        },
        {
          title:"news",
          linkTo:"#",
          isClicked:false
        },
        {
          title:"shop",
          linkTo:"#",
          isClicked:false
        },
      ]
    }
  },

}

</script>

<style lang="scss" scoped>
@import "../assets/style/utils";
@import "../assets/style/mixins";
@import "../assets/style/vars";
  header{
    background-color: white;
    margin:20px 0;
    div{
      display: flex;
      justify-content: space-between;
      nav{
        display: flex;
        align-items: center;
        li{
          position: relative;
          top: 0;
          left: 0;
          display: inline-block;
          a{
            @include headeNavText();
            margin: 0 15px;
            &:hover{
            color:$principal-color;
            cursor: pointer;
            }
          }
        }
      }

    }
  }
</style>