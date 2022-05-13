<template>

  <div>

  <header-layout> </header-layout>

  <main-layout> </main-layout>

  <footer-layout> </footer-layout>

  </div>

</template>

<script>
import FooterLayout from './components/FooterLayout.vue';
import HeaderLayout from './components/HeaderLayout.vue';
import MainLayout from './components/MainLayout.vue';


export default {
  name: 'App',
  components: {
    HeaderLayout,
    MainLayout,
    FooterLayout,

  }
}
</script>

<style lang="scss">
@import "./assets/style/general";
@import "./assets/style/vars";
@import "./assets/style/utils";

</style>
