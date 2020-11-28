<template>
  <div id="app">
        <MainSector/>
  </div>
</template>

<script>

import MainSector from './components/MainSector'

export default {
  name: 'App',
  components: {
    MainSector,
   
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
