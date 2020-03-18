<template>
  <div class="columns">
    <div class="column"></div>
    <div class="column is-four-fifths">
      <div id="app">
        <div id="nav">
          <Navbar/>
        </div>
        <router-view/>
      </div>
    </div>
    <div class="column"></div>
  </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue'
export default {
  components:{
    Navbar
  }
}
</script>
<style lang="scss">
@import url('https://fonts.googleapis.com/css?family=Libre+Baskerville:400,700|Nanum+Gothic:400,700&display=swap');
@import "~bulma/css/bulma.css";

#app{
  font-family: libre baskerville,Georgia,serif;
  -webkit-font-smoothing: antialiased;
  
}

// $font-family: libre baskerville,Georgia,serif;
// #app {
//   font-family: Avenir, Helvetica, Arial, sans-serif;
//   -webkit-font-smoothing: antialiased;
//   -moz-osx-font-smoothing: grayscale;
//   text-align: center;
//   color: #2c3e50;
// }

// #nav {
//   padding: 30px;
// }

// #nav a {
//   font-weight: bold;
//   color: #2c3e50;
// }

// #nav a.router-link-exact-active {
//   color: #42b983;
// }
</style>
