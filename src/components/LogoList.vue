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
        { url: require('@/assets/images/logos/vue.png'), alt: 'Vue.js' },
        {
          url: require('@/assets/images/logos/javascript.png'),
          alt: 'JavaScript',
        },
        { url: require('@/assets/images/logos/mysql.png'), alt: 'MySQL' },
        { url: require('@/assets/images/logos/node.png'), alt: 'Node.js' },
        { url: require('@/assets/images/logos/laravel.png'), alt: 'Laravel' },
        { url: require('@/assets/images/logos/sass.png'), alt: 'Sass' },
        { url: require('@/assets/images/logos/html5.png'), alt: 'HTML5' },
        { url: require('@/assets/images/logos/css3.png'), alt: 'CSS3' },
        { url: require('@/assets/images/logos/php.png'), alt: 'PHP' },
        { url: require('@/assets/images/logos/rest.png'), alt: 'REST API' },
        {
          url: require('@/assets/images/logos/wordpress.png'),
          alt: 'Wordpress',
        },
        { url: require('@/assets/images/logos/jquery.png'), alt: 'jQuery' },
        {
          url: require('@/assets/images/logos/bootstrap.png'),
          alt: 'Bootstrap',
        },
        {
          url: require('@/assets/images/logos/element.png'),
          alt: 'Element UI',
        },
        {
          url: require('@/assets/images/logos/puppeteer.png'),
          alt: 'Puppeteer',
        },
        { url: require('@/assets/images/logos/git.png'), alt: 'Git' },
        { url: require('@/assets/images/logos/figma.png'), alt: 'Figma' },
        { url: require('@/assets/images/logos/vscode.png'), alt: 'VS Code' },
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
