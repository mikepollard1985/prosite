<template>
	<div
		id="psite-about"
		class="psite-about">
		<div class="psite-about-background">
			About.
		</div>
	</div>
</template>

<script>
	export default {
		name: 'psite-about',
		data() {
			return {}
		}
	}
</script>

<style lang="scss">
	.psite-about {
		position: fixed;
		width: 100%;
		height: 100%;
		top: 100%;
		z-index: 1;

		.psite-about-background {
			width: 100%;
			height: 100%;
			text-align: center;
			color: black;
		}
	}
</style>
