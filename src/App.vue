<template>
  <div id="app">
    <x-header>798</x-header>
    <alert v-model="show" title="测试标题" content="测试内容"></alert>
    <img src="assets/logo.png">
    <router-view></router-view>
  </div>
</template>

<script>
  import { XHeader, Alert } from 'vux'

  export default {
    name: 'app',
    data () {
      return {
        show: true
      }
    },
    components: {
      XHeader,
      Alert
    }
  }
</script>

<style>
  body {
    margin: 0;
  }

  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
  }
</style>
