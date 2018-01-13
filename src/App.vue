<template>
  <div id="app">
    <LeftSide/>
    <RightSide/>
  </div>
</template>

<script>
import LeftSide from './components/LeftSide'
import RightSide from './components/RightSide'

export default {
  name: 'app',
  components: {
    LeftSide,
    RightSide
  }
}
</script>

<style>
html, body {
  margin: 0;
}
#app {
  font-family: 'Merriweather', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #000;
}
</style>
