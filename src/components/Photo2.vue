<template>
	<div class="img">
		<div class="title">FREELIFT</div>
		<div class="right"></div>
		<div class="subTitle">Men's basics</div>
		<div class="rec"></div>
		<div class="border"></div>
		<div class="number">02</div>


	</div>


</template>

<script>
	export default {

	}
</script>

<style scoped lang="scss">
	.img {
		display: inline-block;
		position: relative; // z-index: 1;
		background: url("./p2.jpg");
		width: 240px;
		height: 220px;
		background-size: cover;
		background-position: center center;
		margin: 10px 20px;
		margin-top: 150px;
		&>* {

			position: absolute;
			z-index: -1;
		}
	}

	.title {
		position: absolute;
		bottom: -73px;
		left: 120px;
		font-size: 48px;
		font-weight: bold;
	}

	.subTitle {
		position: absolute;
		font-size: 24px;
		font-style: italic;
		font-weight: bold;
		position: absolute;
		top: -28px;
		left: -5px;
		z-index: 1;
	}

	.rec {
		background-color: #50E3C2;
		left: 60px;
		bottom: 50px;
	}

	.border,
	.rec {
		width: 240px;
		height: 200px;
	}

	.border {
		border: 20px solid #50E3C2;
		left: 120px;
		bottom: 100px;
	}

	.number {
		font-size: 48px;
		font-weight: bold;
		top: -82px;
		right: -114px;
	}
</style>