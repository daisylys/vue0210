<template>
  <div id="app">
    <ul class="navbar">
      <!-- 使用 router-link 组件来导航. 通过传入 `to` 属性指定链接. -->
      <router-link tag="li" to="/about">about</router-link>
      <router-link tag="li" to="/">Home</router-link>
      <router-link tag="li" to="/my">My</router-link>
    </ul>
    <!-- 路由出口:路由匹配到的组件将渲染在这里 -->
    <router-view></router-view>
  <p>aaaaaaa</p>
    <el-button>el-button</el-button>
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "app",
  components: {
    HelloWorld
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
ul{
  display: flex;
}
li {
  flex: 1;
  font-size: 12px;
  list-style: none;
}
.router-link-exact-active.router-link-active {
  color: #ffcccc;
}
</style>
