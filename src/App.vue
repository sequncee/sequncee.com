<template>

  <div id="app">
    <Header></Header>
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div> -->
    <router-view />
    <!-- <Footer></Footer> -->
  </div>
</template>

<script>
import "normalize.css/normalize.css";
import Header from "@/components/common/Header0";
// import Footer from "@/components/common/Footer";
// import Head from "@/components/common/Head";

export default {
  name: "Top",
  components: {
    Header
    // Head
    // ,
    // Footer
  }
};
</script>
<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  height: calc(100vh);
}
body {
  margin: 0;
  // test  must delete
  // background-color: #42b983;
  // test must del
}
#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
