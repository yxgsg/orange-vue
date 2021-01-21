<template>
  <div class="about">
    <h1>This is an Test page</h1>
  </div>
  <div id="app">
    <h2>{{ msg }}</h2>
    <br />
    这是一个根组件
    <h3>姓名：{{ userObj.name }} 性别：{{ userObj.sex }}</h3>
  </div>

</template>

<script lang="ts">
export default {
  name: "app",
  data() {
    return {
      msg: "你好，vue",
      userObj: {
        name: "张三",
        sex: "男"
      }
    };
  }
};

</script>
<style>
h2{
  font-family: "Courier New", sans-serif;
  font-size: 100px;
  background: aquamarine;
}
</style>