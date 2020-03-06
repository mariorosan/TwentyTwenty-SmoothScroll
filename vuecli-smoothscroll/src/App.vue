<template>
  <div id="app">
    <HelloWorld />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Roboto:100,300,400,500,700,900&display=swap');

* {
  margin: 0;
  padding: 0;
}

html {
  scroll-behavior: smooth;
  overflow-y: scroll;
  overflow: hidden;
  scroll-snap-type: y mandatory;
}

body {
  height: 100vh;
  font-family: 'Roboto', sans-serif;
  font-weight: 100;
  color: #f4f4f4;
}
</style>
