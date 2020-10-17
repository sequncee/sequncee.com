<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png" /> -->
    <HelloWorld />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "Home",
  components: {
    HelloWorld
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style  lang="scss">
.home {
  background: #3f3f41;
  position: relative;
  display: block;
}

// article, aside, details, figcaption, figure, footer, header, hgroup, main, menu, nav, section, summary {
//     display: block;
// }
* {
  max-height: 1000000px;
}
*,
::before,
::after {
  box-sizing: inherit;
}
</style>
