 //
<HelloWorld msg="Welcome to Your Vue.js App" />
<template>
	<div id="app">
		<div class="subtitle">CCCLOTHES</div>
		<div class="title">MEN'S TOPS</div>
		<div class="row">
			<Photo1 />
			<Photo2 />
		</div>
		<div class="row" :style="{ 'padding-top': '150px'}">
			<Photo3 />
			<Photo4 />
		</div>
		<div class="row"  :style="{'justify-content':'flex-start', 'padding-top': '150px'}">
			<Photo5 />
		</div>
		<div class="row" :style="{ 'padding-top': '150px'}">
			<Photo6 />
			<Photo7 />
		</div>

	</div>
</template>

<script>
	// import HelloWorld from './components/HelloWorld.vue'
	import Photo1 from './components/Photo1.vue';
	import Photo2 from './components/Photo2.vue';
	import Photo3 from './components/Photo3.vue';
	import Photo4 from './components/Photo4.vue';
	import Photo5 from './components/Photo5.vue';
	import Photo6 from './components/Photo6.vue';
	import Photo7 from './components/Photo7.vue';
	export default {
		name: 'app',
		components: {
			Photo1,
			Photo2,
			Photo3,
			Photo4,
			Photo5,
			Photo6,
			Photo7,
		}
	}
</script>

<style lang="scss" scoped>
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
		.row {
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