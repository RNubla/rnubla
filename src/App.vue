<template>
  <div class="columns">
    <div class="column"></div>
    <div class="column is-four-fifths">
      <div id="app">
        <div id="nav">
          <Navbar/>
        </div>
        <router-view/>
        <footer class="footer">
          <div class="content has-text-centered">
            <Footer/>
          </div>
        </footer>
      </div>
    </div>
    <div class="column"></div>
  </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue'
import Footer from '@/components/Footer.vue'
export default {
  components:{
    Navbar,
    Footer
  }
}
</script>
<style lang="scss">
$footer-background-color: white;
// $title-family: libre baskerville,Georgia,serif;
@import url('https://fonts.googleapis.com/css?family=Libre+Baskerville:400,700|Nanum+Gothic:400,700&display=swap');
@import "~bulma/css/bulma.css";

#app{
  font-family: libre baskerville,Georgia,serif;
  -webkit-font-smoothing: antialiased;
  
}
.footer{
  background-color: white;
}
</style>
