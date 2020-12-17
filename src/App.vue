<template>
  <el-container id="app">
    <el-main>
      <MainBanner />
      <InfoCard />
      <LogoList />
    </el-main>
    <el-footer><p>&#169; Vera Goerisch</p></el-footer>
  </el-container>
</template>

<script>
import MainBanner from './components/MainBanner';
import InfoCard from './components/InfoCard';
import LogoList from './components/LogoList';
export default {
  name: 'App',
  components: {
    MainBanner,
    InfoCard,
    LogoList,
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Source+Sans+Pro:wght@300;400;600;700&display=swap');
body {
  margin: 0;
}
#app,
.el-tooltip__popper {
  font-family: 'Source Sans Pro', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #313f47;
}
.el-tooltip__popper {
  font-size: 14px !important;
}
</style>

<style scoped>
.el-main {
  margin: 0;
  padding: 0;
}
.el-footer p {
  margin: 20px 0 0;
}
</style>
