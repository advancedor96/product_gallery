<template>
	<div class="img">
		<div class="title">EDITION</div>
		<div class="subTitle">Men’s shirts</div>
		<div class="rec"></div>
		<div class="border"></div>
		<div class="number">07</div>
	</div>
</template>
<script>
	export default {

	}
</script>

<style scoped lang="scss">
	* {
		box-sizing: border-box;
	}

	.img {
		margin: 60px 120px 0px 30px;
		display: inline-block;
		position: relative;
		background: url("./p7.jpg");
		width: 240px;
		height: 400px;
		background-size: cover;
		background-position: center center;
		font-family: Roboto-Black;
		;
		&>* {
			position: absolute;
			z-index: -1;

		}
	}

	.title {
		// width: 336px;
		height: 48px;
		line-height: 48px;
		position: absolute;
		left: 240px;
		top: -50px;
		font-size: 48px;
		font-weight: bold;
		text-shadow: 0px -21px rgba(0, 0, 0, 0.3), 0px -35px rgba(0, 0, 0, 0.1);
		z-index: 0;
		transform-origin: 0 100%;
		transform: rotate(90deg);
	}

	.subTitle {
		position: absolute;
		font-family: Roboto;
		font-size: 24px;
		font-style: italic;
		font-weight: bold;
		position: absolute;
		top: -28px;
		left: 0;
		z-index: 1;
	}

	.border {
		width: 240px;
		height: 400px;
		display: inline-block;
		top: -50px;
		left: 60px;
		border: 20px solid #50E3C2;
		z-index: -1;
	}

	.rec {
		width: 240px;
		height: 200px;
		display: inline-block;
		bottom: 0;
		right: -120px;
		background-color: #50E3C2;
		z-index: -1;
	}

	.number {
		font-size: 48px;
		font-weight: bold;
		right: -120px;
		bottom: 0;
		line-height: 48px;
	}
</style>