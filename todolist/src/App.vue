<template>
  <div>
    <NavBar />
    <button class="btn btn-primary">点击我</button>
    <button class="btn btn-wide">Wide</button>
    <PageContent />
    <AppFooter />
  </div>
</template>

<script>
import NavBar from './components/NavBar.vue';
import PageContent from './components/PageContent.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  name: 'App',
  components: {
    NavBar,
    PageContent,
    AppFooter,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

body {
    margin: 0; /* 去除浏览器默认边距 */
}
</style>