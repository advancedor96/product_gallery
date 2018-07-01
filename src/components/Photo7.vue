<template>
	<div class="photo7-container">

		<div class="img">
			<div class="title">EDITION</div>
			<div class="subTitle">Men’s shirts</div>
			<div class="rec"></div>
			<div class="border"></div>
			<div class="number">07</div>
		</div>
	</div>
</template>
<script>
	export default {

	}
</script>

<style scoped lang="scss">
	$pc: 960px;
	$padMax: 959px;
	$padMin: 481px;
	$phoneMax:480px;

	@mixin pc() {
		@media all and(max-width: $pc) {
			@content;
		}
	}

	@mixin pad() {
		@media all and(min-width: $padMin) and (max-width: $padMax) {
			@content;
		}
	}

	@mixin mobile() {
		@media all and(max-width: $phoneMax) {
			@content;
		}
	}

	.photo7-container {
		display: inline-block;
		margin-top: 60px;
		order: 1;
		@include pad() {
			order: 2;
		}
		@include mobile() {
			order: 2;
		}
	}

	.img {
		margin: 0;

		margin-top: 50px;
		margin-left: 0px;
		margin-right: 120px;

		display: inline-block;
		position: relative;
		background: url("./p7.jpg");
		width: 240px;
		height: 400px;
		background-size: cover;
		background-position: center center;
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