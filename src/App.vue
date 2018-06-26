 //
<HelloWorld msg="Welcome to Your Vue.js App" />
<template>
	<div id="app">
		<div class="subtitle">CCCCCLOTHES</div>
		<div class="title">MENS'S TOPS</div>
		<div class="row">
		<Photo1 />
		<Photo2 />

		</div>
	</div>
</template>

<script>
	// import HelloWorld from './components/HelloWorld.vue'
	import Photo1 from './components/Photo1.vue';
	import Photo2 from './components/Photo2.vue';
	export default {
		name: 'app',
		components: {
			Photo1,
			Photo2
		}
	}
</script>

<style lang="scss">
	* {
		box-sizing: border-box;
	}

	html,
	body {
		font-family: 'Roboto', sans-serif;

	}

	#app {
		.subtitle {
			font-size: 20px;
			background-color: black;
			color: white;
			width: 191px;
			height: 27px;
			padding: 2px 4px;
			text-align: center;
			margin: 0 auto;
		}
		.title {
			text-align: center;
			font-size: 72px;
			height: 85px;
			font-weight: bold;
			margin-top: 9px;
		}
		.row{
			margin-top: 34px;
			display: flex;
			flex-wrap: wrap;
			justify-content: center;
		}
		/* font-family: 'Roboto', sans-serif;; */
		/* font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px; */
	}
</style>