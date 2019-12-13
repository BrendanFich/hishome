<template>
  <div id="app">
    <Home/>
  </div>
</template>

<script>
import Home from './components/Home'

export default {
  name: 'App',
  components: {
    Home
  }
}
</script>

<style>
html, body {
  height: 100%;
  margin: 0;
  padding: 0;
  font-family: "Microsoft YaHei", "微软雅黑", Arial, sans-serif
}
</style>
