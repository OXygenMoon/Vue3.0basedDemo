<template>
    <main>
      <h1>欢迎来到我的网站！</h1>
      <p>这里是网站的主要内容。</p>
    </main>
  </template>
  
  <script>
  export default {
    name: 'PageContent',
  };
  </script>
  
  <style scoped>
  main {
    padding: 20px;
    min-height: 400px; /* 设置最小高度，避免页脚浮动到内容上方 */
  }
  </style>