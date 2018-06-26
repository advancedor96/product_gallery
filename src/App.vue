   //  <HelloWorld msg="Welcome to Your Vue.js App"/>
<template>
  <div id="app">
		<Photo1 />
		<Photo2 />
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Photo1 from './components/Photo1.vue';
import Photo2 from './components/Photo2.vue';
export default {
  name: 'app',
  components: {
    Photo1, Photo2
  }
}
</script>

<style>
*{
	box-sizing: border-box;
}
html, body{
	font-family: 'Roboto', sans-serif;
	
}
#app {
	/* font-family: 'Roboto', sans-serif;; */
  /* font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px; */
}
</style>
