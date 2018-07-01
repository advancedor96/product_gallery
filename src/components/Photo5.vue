<template>
	<div class="img">
		<div class="title">SWEATSHIRTS</div>
		<div class="subTitle">Men’s jacket</div>
		<div class="slash"></div>
		<div class="border"></div>
		<div class="number">05</div>
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
		margin-left: 280px;
		display: inline-block;
		position: relative;
		background: url("./p5.jpg"); // transform: scaleX(-1);
		width: 240px;
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
		right: 153px;
		top: 53px;
		font-size: 48px;
		font-weight: bold;
		text-shadow: 0px -21px rgba(0, 0, 0, 0.3), 0px -35px rgba(0, 0, 0, 0.1);
		z-index: 0;
	}

	.slash {
		position: absolute;
		display: inline-block;
		right: 180px;
		top: -50px;
		width: 240px;
		height: 100px;
		background: linear-gradient(-45deg, #50E3C2 8%, transparent 8%,
		transparent 16%, #50E3C2 16%,
		#50E3C2 24%, transparent 24%,
		transparent 32%, #50E3C2 32%,
		#50E3C2 40%, transparent 40%,
		transparent 48%, #50E3C2 48%,
		#50E3C2 56%, transparent 56%,
		transparent 64%, #50E3C2 64%,
		#50E3C2 72%, transparent 72%,
		transparent 80%, #50E3C2 80%,
		#50E3C2 88%, transparent 88%,
		transparent 96%, #50E3C2 96%); // 比較直覺的方式，哈
		z-index: -1;

	}

	.subTitle {
		font-family: Roboto;
		font-size: 24px;
		width: 100%;
		font-style: italic;
		font-weight: bold;
		position: absolute;
		top: 0;
		left: 240px;
		z-index: 1;
	}

	.border {
		width: 240px;
		height: 100px;
		display: inline-block;
		top: 150px;
		right: 120px;
		border: 20px solid #50E3C2;
		z-index: -1;
	}

	.number {
		font-size: 48px;
		font-weight: bold;
		right: 304px;
		bottom: 0;
		line-height: 48px;
	}
</style>