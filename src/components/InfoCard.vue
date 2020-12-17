<template>
  <el-card
    ><el-row :gutter="20"
      ><el-col :md="12" :xs="24"
        ><h3>About</h3>
        <p>
          Hello! My name is Vera Goerisch and I am a web developer who loves
          learning, challenges, and bringing ideas to life. Originally from
          Russia, I currently reside in sunny San Diego (and I couldn't be
          happier about it). When I am not writing code, I can be found spending
          time with my daughter, swing dancing, hiking, backpacking, or
          otherwise exploring the beautiful outdoors. I also love traveling
          around the world and experiencing other cultures.
        </p>
        <p>
          My professional goal is to never stop learning and continue expanding
          my skill set (check the list below for my current skills and some of
          my favorite technology).
        </p>
        <p>
          I'm always looking for new connections and interesting opportunities.
          Don't hesitate to contact me if you'd like to get in touch!
        </p></el-col
      ><el-col :md="12" :xs="24"
        ><h3>Basic Information</h3>
        <p><span class="description">Email:</span>contact@veragoerisch.com</p>
        <p><span class="description">Location:</span>San Diego, CA</p>
        <p><span class="description">Languages:</span>English, Russian</p>
        <p>
          <span class="description">Available for new opportunities:</span>Yes
        </p>
        <p>
          <span class="description">Current framework of choice:</span
          ><el-link href="https://vuejs.org/" target="_blank" class="vue-link"
            >Vue.js &#10084;</el-link
          >
        </p></el-col
      ></el-row
    ></el-card
  >
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
.el-card {
  margin: 30px auto;
  padding-bottom: 10px;
  max-width: 90%;
  p {
    text-align: justify;
    padding: 0 30px;
    .description {
      font-weight: 600;
      margin-right: 10px;
    }
  }
  .el-link.vue-link {
    font-size: 16px;
    vertical-align: baseline;
    color: #41b883;
  }
}
</style>
