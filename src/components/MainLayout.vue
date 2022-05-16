<template>
    <main>
      <main-component-jumbo></main-component-jumbo>
      <div class="container">
        <p class="current-series-special-div">current series</p>
        <main-component-card
        v-for="(comic, index) in dcComics" :key="`comic-${index}`"
        :comic ="comic"
        ></main-component-card>
      </div>
    </main>
</template>

<script>
import dcComics  from '../assets/data/dcComics'
import MainComponentCard from './MainComponentCard.vue'
import MainComponentJumbo from './MainComponentJumbo.vue'
export default {
  name: "MainLayout",
  components: { MainComponentJumbo, MainComponentCard },
  data() {
    return {
      dcComics
    }
  },
}
</script>

<style lang="scss" scoped>
@import "../assets/style/utils";
@import "../assets/style/mixins";
@import "../assets/style/vars";
  main{
    background-color: #1c1c1c;
    .current-series-special-div{
      width: fit-content;
      padding: 13px 20px;
      font-weight: 600;
      text-transform: uppercase;
      color: white;
      background-color: $principal-color;
    }
}

</style>