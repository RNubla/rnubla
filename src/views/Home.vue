<template>
  <div class="home">
    <div class="container">
      
      <section class="hero">
        <div class="hero-body">
          <h1 class="title">
            <HelloWorld msg="Hello, my name is Robert. I am a Computer Science Major at West Chester University"/>
          </h1>
        </div>
      </section>
    
    </div>
    <div class="container">
      
      <figure class="image is-3by1">
        <!-- <img src="https://source.unsplash.com/xrVDYZRGdw4/1920x1080" alt="" srcset=""> -->
        <img src="../assets/laptop.jpg" alt="" srcset="">
      </figure>
    
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
