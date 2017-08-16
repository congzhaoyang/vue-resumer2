<template>
  <div id="app">
    <header>
      <Topbar></Topbar>
    </header>
    <div class="main">
      <ResumerEditor></ResumerEditor>
      <ResumerPreview></ResumerPreview>
    </div>
  </div>
</template>

<script>
import Topbar from './components/Topbar'
import ResumerEditor from './components/ResumeEditor'
import ResumerPreview from './components/ResumePreview'
import 'normalize.css'

export default {
  name: 'app',
  components: {
    Topbar, ResumerEditor, ResumerPreview
  }
}
</script>

<style lang="scss">
#app {
  width: 1220px;
  height: 100vh;
  background: #EDEDED;
  margin: 0 auto;
  display: flex;
  flex-direction: column;
  header {
    #Topbar {
      background: #DDDDDD;
      height: 64px;
      width: 100%;
    }
  }
  .main {
    flex-grow: 1;
    border: 1px solid red;
    display: flex;
    margin-top: 16px;
    #ResumerEditor {
      width: 36%;
      margin-right: 8px;
    }
    #ResumerPreview {
      flex: 1;
      margin-left: 8px;
    }
  }
}
</style>
