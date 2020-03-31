<template>
  <div id="app">
    <div id="nav">
      <!-- <Navbar /> -->
    </div>
    <router-view />
    <footer class="footer">
      <div class="content has-text-centered">
        <Footer />
      </div>
    </footer>
  </div>
</template>

<script>
// import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";
export default {
  components: {
    // Navbar,
    Footer
  }
};
</script>
<style lang="scss">
$footer-background-color: white;
$panel-block-color	: white;
// $title-family: libre baskerville,Georgia,serif;
@import url("https://fonts.googleapis.com/css?family=Libre+Baskerville:400,700|Nanum+Gothic:400,700&display=swap");
@import "~bulma/css/bulma.css";

#app {
  font-family: libre baskerville, Georgia, serif;
  -webkit-font-smoothing: antialiased;
}
.footer {
  background-color: white;
}
html,
body {
  // font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen-Sans, Ubuntu, Cantarell, "Helvetica Neue", sans-serif;
  // font-size: 14px;
  background: #f0f2f4;
}
</style>
