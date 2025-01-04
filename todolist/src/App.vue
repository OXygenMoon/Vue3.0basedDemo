<template>
  <div>
    <NavBar />
    <PageContent />
    <AppFooter />
  </div>
</template>


<script>
import NavBar from "./components/NavBar.vue";
import PageContent from "./components/PageContent.vue";
import AppFooter from "./components/AppFooter.vue";
import { onMounted, watchEffect } from "vue";

export default {
  name: "App",
  components: {
    NavBar,
    PageContent,
    AppFooter,
  },
  setup() {
    onMounted(() => {
      document.documentElement.setAttribute('data-theme', localStorage.getItem('data-theme') || "cupcake");
      watchEffect(() => {
        const theme = localStorage.getItem('data-theme');
        if (theme) {
          document.documentElement.setAttribute('data-theme', theme);
        }
      });
    });

    return {};
  }
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
