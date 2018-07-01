<template>
	<div class="photo6-container">
		<div class="img">
			<div class="title">VINTAGE DENIM</div>
			<div class="subTitle">Men’s classic</div>
			<div class="rec"></div>
			<div class="border"></div>
			<div class="number">06</div>
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

	.photo6-container {
		display: inline-block;
		margin-top: -170px;
		order: 2;
		@include pad() {
			margin-top: 40px;
			order: 1;
		}
		@include mobile() {
			margin-top: 40px;
			order: 1;
		}
	}

	.img {
		display: inline-block;
		position: relative;
		background: url("./p6.jpg");
		width: 480px;
		height: 400px;
		background-size: cover;
		background-position: center center;
		font-family: Roboto-Black;
		margin: 0;
		margin-top: 80px;
		margin-bottom: 50px;
		margin-left: 60px;

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
		bottom: -28px;
		left: 170px;
		z-index: 1;
	}

	.border {
		width: 480px;
		height: 200px;
		display: inline-block;
		bottom: -50px;
		left: 0;
		border: 20px solid #50E3C2;
		z-index: -1;
	}


	.rec {
		width: 240px;
		height: 200px;
		display: inline-block;
		bottom: 0;
		left: -60px;
		background-color: #50E3C2;
		z-index: -1;
	}

	.number {
		font-size: 48px;
		font-weight: bold;
		right: 480px;
		top: 151px;
		bottom: 0;
		line-height: 48px;
	}
</style>