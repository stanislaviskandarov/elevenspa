<template>
  <div id="app">
    <Navbar />
    <HomePage />
    <Footer />
  </div>
</template>

<script>
import HomePage from "./components/HomePage";
import Navbar from "./components/Navbar";
import Footer from "./components/Footer";

export default {
  name: "App",
  data() {
    return {};
  },
  components: {
    HomePage,
    Navbar,
    Footer,
  },
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
