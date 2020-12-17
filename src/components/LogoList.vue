<template>
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

<style scoped lang="scss">
.logo {
  margin: 25px 0;
  .el-image {
    width: 100px;
    height: 100px;
  }
}
</style>
