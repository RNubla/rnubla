<template>
  <div class="home">
    <div class="container">
      
      <section class="hero">
        <div class="hero-body">
          <h1 class="title">
            <div class="columns">
              <div class="column "></div>
              <div id="hero-text" class="column is-two-thirds">
                <HelloWorld msg="Hello, my name is Robert. I am a Computer Science Major at West Chester University"/>
              </div>
              <div class="column"></div>
            </div>
          </h1>
        </div>
      </section>
    
    </div>
    <div class="container">
      
      <figure class="image is-3by1">
        <img src="../assets/laptop.jpg" alt="" srcset="">
      </figure>
    
    </div>
    <div class="container">
      <div class="columns">
        <div class="column is-full">
          <div class="columns">
            <div class="column is-two-fifths"></div>
            <div class="column">
              <HelloWorld msg='About'/>
            </div>
            <div class="column"></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>

<style scoped>
#hero-text{
  text-align: center
}
</style>
