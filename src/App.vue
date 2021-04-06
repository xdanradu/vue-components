<template>
  <div id="app">
    <Banner msg="Some message from outside"></Banner>
    <MenuOption url="http://google.com" option="Google"></MenuOption>
    <Photo path="https://homepages.cae.wisc.edu/~ece533/images/airplane.png"></Photo>
  </div>
</template>

<script>
import Banner from './components/Banner.vue'
import Photo from './components/Photo.vue'
import MenuOption from './components/MenuOption';

export default {
  name: 'App',
  components: {
    Banner, Photo, MenuOption
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
  margin: 0;
  padding: 0;
}
</style>
