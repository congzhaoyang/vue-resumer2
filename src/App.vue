<template>
  <div id="app">
    <img src="./assets/logo.png">
    <router-view></router-view>
      <Topbar/>
      <ResumerEditor/>
      <ResumerPreview/>
  </div>
</template>

<script>
import Topbar from './components/Topbar'
import ResumerEditor from './components/ResumeEditor'
import ResumerPreview from './components/ResumePreview'

export default {
  name: 'app',
  components: {
    Topbar, ResumerEditor, ResumerPreview
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
