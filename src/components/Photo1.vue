<template>
	<div class="container">
		<div class="title">LINEN BLAZER</div>
		<div class="img"></div>
		<div class="right"></div>
		<div class="left_bottom">01</div>
		<div class="slash_block"></div>
		<div class="right_down">Men's outfit</div>

	</div>
</template>

<script>
	export default {

	}
</script>

<style scoped lang="scss" >
	.container {
		display: inline-block;
		width: 540px;
		height: 500px;
		font-weight: bold;
		position: relative;
		margin: 10px 20px;
		.title {
			z-index: 1;
			position: absolute;
			top: 35px;
			font-size: 48px;
			line-height: 48px;
			text-shadow: 0px -21px rgba(0, 0, 0, 0.3), 0px -35px rgba(0, 0, 0, 0.1)
		}
		.img {
			z-index: 0;
			position: absolute;
			top: 49px;
			background: url("./p1.jpg");
			width: 480px;
			height: 400px;
			background-size: cover;
			background-position: center center;
		}
		.right_down {
			position: absolute;
			right: 58px;
			bottom: 0;
			z-index: 2;
			transform-origin: 100% 100%;
			transform: rotate(90deg);
		}

		.slash_block {
			position: absolute;
			left: 60px;
			bottom: 0px;
			z-index: 1;
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
		}

		.left_bottom {
			position: absolute;
			bottom: 0;
			left: 0;
			font-size: 48px;
			width: 56px;
			height: 48px;
			line-height: 48px;
		}

		.right {
			position: absolute;
			z-index: -1;
			top: 0;
			right: 0;
			width: 240px;
			height: 200px;
			border: 20px solid #50E3C2;

		}
	}
</style>