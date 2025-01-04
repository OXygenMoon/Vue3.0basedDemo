<template>
    <nav>
      <ul>
        <li><a href="#">首页</a></li>
        <li><a href="#">关于我们</a></li>
        <li><a href="#">联系我们</a></li>
      </ul>
    </nav>
  </template>
  
  <script>
  export default {
    name: 'NavBar',
  };
  </script>
  
  <style scoped>
  nav {
    background-color: #f0f0f0;
    padding: 10px;
  }
  
  ul {
    list-style: none;
    margin: 0;
    padding: 0;
    display: flex;
  }
  
  li {
    margin-right: 20px;
  }
  </style>