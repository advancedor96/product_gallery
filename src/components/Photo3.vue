<template>
	<div class="img">
		<div class="title">SUPER SKINNY</div>
		<div class="subTitle">Men’s pattern shirts</div>
		<div class="rec"></div>
		<div class="border"></div>
		<div class="number">03</div>
	</div>
</template>
<script>
	export default {

	}
</script>

<style scoped lang="scss">
	*{
		box-sizing: border-box;
	}
	.img {

		display: inline-block;
		position: relative;
		background: url("./p3.jpg");
		width: 480px;
		height: 200px;
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
		right: 0;
		top: -48px;
		font-size: 48px;
		font-weight: bold;
		text-shadow: 0px -21px rgba(0, 0, 0, 0.3), 0px -35px rgba(0, 0, 0, 0.1);
		z-index: 0;
	}

	.subTitle {
		position: absolute;
		font-family: Roboto;
		font-size: 24px;
		font-style: italic;
		font-weight: bold;
		position: absolute;
		bottom: -31px;
		left: 31px;
		z-index: 1;
	}

	.rec {
		width: 240px;
		height: 50px;
		display: inline-block;
		top: -50px;
		left: 0;
		background-color: #50E3C2;
		z-index: -1;
	}

	.border {
		width: 240px;
		height: 200px;
		border: 20px solid #50E3C2;
		z-index: -1;
		right: -60px;
		bottom: -50px;
	}
	.number {
		font-size: 48px;
		font-weight: bold;
		right: -56px;
		bottom: -50px;
		line-height: 48px;
	}
</style>