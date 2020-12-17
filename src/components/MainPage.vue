<template>
  <el-container>
    <el-main>
      <el-row>
        <el-col :span="24"
          ><div class="background">
            <el-avatar
              class="avatar"
              :size="250"
              src="/images/profile.jpg"
            ></el-avatar>
            <h2>Vera Goerisch</h2>
            <h3>Front-End Web Developer</h3>
            <el-row class="buttons">
              <a class="button" href="#" target="_blank"
                ><i class="far fa-envelope"></i
              ></a>
              <a class="button" href="#" target="_blank"
                ><i class="fab fa-linkedin-in"></i
              ></a>

              <a class="button" href="#" target="_blank"
                ><i class="fab fa-github"></i
              ></a>
              <a class="button" href="#" target="_blank"
                ><i class="fas fa-file-download"></i
              ></a>
            </el-row>
          </div>
        </el-col>
      </el-row>
      <el-card
        ><el-row
          ><el-col :span="12"
            ><h3>About</h3>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla vel
              ex non mi tempus egestas. Integer mollis nec lorem eu cursus. In
              tempus, eros id venenatis aliquam, sapien ipsum pulvinar tortor,
              nec aliquet ante velit et nulla. Mauris lacus mauris, tempus sit
              amet iaculis dignissim, sodales ac ligula. Sed eu vulputate lorem.
              Ut eget purus malesuada, vestibulum libero vitae, pulvinar nulla.
              In in neque nibh. Phasellus faucibus dictum molestie. Vivamus sit
              amet vulputate nibh, quis congue nibh. Fusce scelerisque lorem non
              dignissim ultricies. Integer dolor est, efficitur non finibus
              quis, ornare et urna.
            </p></el-col
          ><el-col :span="12"
            ><h3>Basic Information</h3>
            <p>Email: contact@veragoerisch.com</p>
            <p>Phone: (619) 735-6183</p>
            <p>Location: San Diego, CA</p>
            <p>Language: English, Russian</p></el-col
          ></el-row
        ></el-card
      >
      <el-row
        ><el-col
          :lg="4"
          :sm="8"
          :xs="12"
          class="logo"
          v-for="(logo, index) in logos"
          :key="index"
          ><el-image
            :src="logo.url"
            :alt="logo.alt"
            fit="scale-down"
          ></el-image></el-col
      ></el-row>
    </el-main>
    <el-footer><p>&#169; Vera Goerisch</p></el-footer>
  </el-container>
</template>

<script>
export default {
  data() {
    return {
      logos: [
        { url: '/images/logos/vue.png', alt: 'Vue.js' },
        { url: '/images/logos/javascript.png', alt: 'JavaScript' },
        { url: '/images/logos/mysql.png', alt: 'MySQL' },
        { url: '/images/logos/node.png', alt: 'Node.js' },
        { url: '/images/logos/laravel.png', alt: 'Laravel' },
        { url: '/images/logos/sass.png', alt: 'Sass' },
        { url: '/images/logos/html5.png', alt: 'HTML5' },
        { url: '/images/logos/css3.png', alt: 'CSS3' },
        { url: '/images/logos/php.png', alt: 'PHP' },
        { url: '/images/logos/rest.png', alt: 'REST API' },
        { url: '/images/logos/wordpress.png', alt: 'Wordpress' },
        { url: '/images/logos/jquery.png', alt: 'jQuery' },
        { url: '/images/logos/bootstrap.png', alt: 'Bootstrap' },
        { url: '/images/logos/element.png', alt: 'Element UI' },
        { url: '/images/logos/puppeteer.png', alt: 'Puppeteer' },
        { url: '/images/logos/git.png', alt: 'Git' },
        { url: '/images/logos/figma.png', alt: 'Figma' },
        { url: '/images/logos/vscode.png', alt: 'VS Code' },
      ],
    };
  },
};
</script>

<style scoped>
.el-main {
  margin: 0;
  padding: 0;
}
.background {
  background: url('/images/background.jpg') no-repeat center center fixed;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
  height: 500px;
  position: relative;
  margin-bottom: 30px;
}
.background h2,
.background h3 {
  color: #fff;
  font-weight: 300;
  text-transform: uppercase;
  letter-spacing: 0.15em;
}
.background h2 {
  font-size: 48px;
  letter-spacing: 6px;
  margin: 0 0 30px;
}
.background h3 {
  font-size: 24px;
  letter-spacing: 3px;
}
.avatar {
  margin: 30px auto 20px;
}
.buttons {
  position: absolute;
  top: 460px;
  width: 100%;
  margin: 0 auto;
}
.button {
  display: inline-block;
  margin: 7px;
  height: 60px;
  width: 60px;
  border-radius: 50%;
  color: #fff;
  background-color: #989898;
  font-size: 30px;
  line-height: 60px;
}
.button:hover,
.button:focus,
.button:active {
  background-color: #858585;
  color: #e7e7e7;
}
.el-card {
  margin: 30px auto;
  max-width: 90%;
}
.logo {
  margin: 25px 0;
}
.logo .el-image {
  width: 100px;
  height: 100px;
}
.el-footer p {
  margin: 20px 0 0;
}
</style>
