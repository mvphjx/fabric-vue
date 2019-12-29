<template>
  <div id="app">
    <Fabric msg="this is a fabric demo" :width=500 :height=300 />
  </div>
</template>

<script>
import Fabric from './components/Fabric.vue'
//import hi from './components/HelloWorld.vue'
export default {
  name: 'app',
  components: {
      Fabric
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
