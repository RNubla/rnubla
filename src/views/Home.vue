<template>
  <div class="home">
    <div class="container">
      <section class="hero">
        <div class="hero-body">
          <h1 class="title">
            <div class="columns">
              <div class="column "></div>
              <div id="hero-text" class="column is-two-thirds">
                <HelloWorld
                  msg="Hello, my name is Robert. I am a Computer Science Major at West Chester University"
                />
              </div>
              <div class="column"></div>
            </div>
          </h1>
        </div>
      </section>
    </div>
    <div class="container">
      <figure class="image is-3by1">
        <img src="../assets/laptop.jpg" alt="" srcset="" />
      </figure>
    </div>
    <body>
      <div class="columns">
        <div class="column"></div>
        <div class="column is-two-thirds">
          <section class="section">
            <div class="container">
              <h1 class="title">About:</h1>
              <p>
                I am currently in my senior year at West Chester University. I am
                persuing my Bachelor's degree in Computer Science and will be graduating
                in the fall of 2020. I've been interested in programming ever since 
                I was introduced to the Unity Game Engine. I like to learn new 
                technologies and I am very motivated to work and improve my programming
                skills. I currently work as an IT Technician at a small IT firm. This 
                position enables me to improve my troubleshooting skills, which can be applied
                to software developement. 
              </p>
            </div>
          </section>
          <section class="section">
            <div class="container">
              <h1 class="title">Languages:</h1>
              <p>
                The languages that I am comfortable using are Java and Python. However, I have been 
                getting myself familiar with Vuejs, CSS and HTML. This website was developed using 
                those three languages. 
              </p>
            </div>
          </section>
        </div>
        <div class="column"></div>
      </div>
    </body>
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

<style scoped>
#hero-text {
  text-align: center;
}
/* .home .container{
  background-image: url('../assets/laptop.jpg');
} */
</style>
