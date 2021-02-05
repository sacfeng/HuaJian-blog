<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="花间"/> -->
    <MainHeader></MainHeader>
    <MainContent></MainContent>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import MainHeader from './components/header/MainHeader.vue'
import MainContent from './components/main/MainContent.vue'
export default {
  name: 'App',
  components: {
    // HelloWorld,
    MainHeader,
    MainContent
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
