 //
<HelloWorld msg="Welcome to Your Vue.js App" />
<template>
	<div id="app">
		<div class="container">

			<div class="subtitle">CCCLOTHES</div>
			<div class="title">MEN'S TOPS</div>

			<div class="row">
				<Photo1 />
				<Photo2 />
			</div>

			<div class="row" :style="{'margin-top': '77px'}">   <!-- :style="{ 'padding-top': '150px'}" -->
				<Photo3 />
				<Photo4 />
			</div>
			<div class="row" :style="{'justify-content':'flex-start'}">
				<Photo5 />
			</div>
			<div class="row67" >
				<Photo6 />
				<Photo7 />
			</div>
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
<style lang="scss">

	html,
	body {
		font-family: 'Roboto', sans-serif;
		margin: 0;
		padding: 0;
		overflow-x: hidden;

	}

	* {
		box-sizing: border-box;
	}
</style>

<style lang="scss" scoped>
	#app {
		width: 100%;
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
			height: 72px;
			font-weight: bold;
			margin-top: 9px;
		}
		.row {
			margin-top: 34px;
			display: flex;
			flex-wrap: wrap;
			justify-content: space-between;
		}
		.row67{
			margin-top: 34px;
			display: flex;
			flex-wrap: wrap;
			justify-content: space-between;
			
		}

	}

	.container {
		max-width: 1040px;
		width: 100%;
		min-width: 500px; // background-color: gray;
		margin: 0 auto;
		padding: 32px;
	}
</style>