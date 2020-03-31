<template>
  <div class="home">
    <section class="hero is-info is-medium is-bold">
      <div class="hero-body">
        <div class="container has-text-centered">
          <h1 class="title article-title">
            Hello, my name is Robert. I am a Computer Science Major at West
            Chester University
          </h1>
        </div>
      </div>
    </section>

    <body>
      <div class="container">
        <section class="articles">
          <div class="column is-half is-offset-one-quarter">
            <div class="card article">
              <div class="card-content">
                <div class="media">
                  <div class="media-content has-text-centered">
                    <div class="content">
                      <p class="title article-title">About Me</p>
                      <div class="tags has-addons level-item">
                        <a
                          href="https://github.com/RNubla"
                          class="tag is-rounded is-success"
                          >GitHub</a
                        >
                        <a
                          href="https://linkedin.com/in/robert-nubla-0b9a64157"
                          class="tag is-rounded is-link"
                          >LinkedIn</a
                        >
                      </div>
                    </div>
                  </div>
                </div>
                <div class="content article-body">
                  <p>
                    I am currently in my senior year at West Chester University.
                    I am persuing my Bachelor's degree in Computer Science and
                    will be graduating in the fall of 2020. I've been interested
                    in programming ever since I tried on making my own games
                    using the Unity Game Engine. I love learn new technologies
                    and I am always motivated to work and improve my skills. I
                    currently work as an IT Technician at a small IT firm. This
                    position enables me to improve my troubleshooting skills,
                    which can be applied to software developement.
                  </p>
                </div>
              </div>
            </div>
          </div>
        </section>
      </div>
      <section class="section">
        <div class="container">
          <section class="articles">
            <div class="column is-half is-offset-one-quarter">
              <div class="card article">
                <div class="card-content">
                  <div class="media">
                    <div class="media-content has-text-centered">
                      <div class="content">
                        <p class="title article-title">
                          Technologies That I Use
                        </p>
                      </div>
                    </div>
                  </div>
                  <div class="content article-body">
                    <div class="content">
                      <ul id="progList">
                        <li v-for="lang in progLang" :key="lang.name">
                          {{ lang.name }}
                        </li>
                      </ul>
                    </div>
                    <p>
                      The technologies that I am comfortable with are Java and
                      Python. However, I have been getting myself familiar with
                      Vuejs, CSS and HTML. This website was developed using
                      those three web technologies. I am dedicated to learn more
                      about web development. As of right now, I am focusing on
                      Front-End developement. In the near future, I will be
                      learning about the Back-End of web developement, My goal
                      is to become a Full-Stack developer.
                    </p>
                  </div>
                </div>
              </div>
            </div>
          </section>
        </div>
      </section>
    </body>
  </div>
</template>

<script scoped>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue";
export default {
  name: "Home",
  // el: "#progList",
  data() {
    return {
      progLang: [
        { name: "Java" },
        { name: "Python" },
        { name: "Javascript" },
        { name: "Firebase" },
        { name: "Github" },
        { name: "Vuejs" }
      ]
    };
  },
  components: {
    // HelloWorld
  }
};
</script>

<style scoped>
#hero-text {
  text-align: center;
}

.hero-body {
  background-image: url("../assets/laptop2.jpg");
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
  height: 500px;
}
.media-center {
  display: block;
  margin-bottom: 1rem;
}
.media-content {
  margin-top: 3rem;
}
.articles {
  margin: 5rem 0;
  margin-top: -200px;
}
.articles .content p {
  line-height: 1.9;
  margin: 15px 0;
}
.article,
.promo-block {
  margin-top: 6rem;
}
.article-title {
  font-size: 2rem;
  font-weight: lighter;
  line-height: 2;
}
.article-subtitle {
  color: #909aa0;
  margin-bottom: 3rem;
}
.article-body {
  line-height: 1.4;
  margin: 0 6rem;
}
.promo-block .container {
  margin: 1rem 5rem;
}
</style>
