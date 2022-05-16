<template>

    <footer>
      <footer-component-first> </footer-component-first>
      <footer-component-second></footer-component-second>
      <footer-component-third></footer-component-third>


    </footer>

</template>

<script>
import FooterComponentFirst from './FooterComponentFirst.vue'
import FooterComponentSecond from './FooterComponentSecond.vue'
import FooterComponentThird from './FooterComponentThird.vue'
export default {
  name: "FooterLayout",
  components : {FooterComponentFirst, FooterComponentSecond, FooterComponentThird}
}
</script>

<style lang="scss" scoped>
@import "../assets/style/utils";
@import "../assets/style/mixins";
@import "../assets/style/vars";
</style>