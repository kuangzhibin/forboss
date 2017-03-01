<template>
  <div id="app">
    <div id="header"></div>
    <div id="main">
      <div id="sidebar">
        <el-menu class="el-menu-vertical-demo">
          <el-menu-item index="2"><router-link tag="li" to="/new">
            <i class="el-icon-menu"></i>new</router-link>
          </el-menu-item>
        </el-menu>
      </div>
      <div id="container">
        <router-view></router-view>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app {
  background: #ddd;
  display: flex;
  flex-direction: column;
  height: 100vh;
}
#header {
  background: #222;
  flex: 0 0 44px;
}
#main {
  background: #fff;
  display: flex;
  flex: 1 1 auto;
}
#sidebar {
  background: #eef1f6;
  flex: 0 0 200px;
}
#container {
  /*background: #ff0;*/
  flex: auto;
  padding: 12px;
  margin: 12px;
  border: 1px solid #ebebeb;;
}
</style>
