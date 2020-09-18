<template>
	<div class="psite-home" id="psite-home">
		<video
			ref="psite_bg_vid"
			class="psite-video-background"
			autoplay muted loop>
			<source src="../assets/video/background_blur.mp4" type="video/mp4"/>
			Sorry, your browser doesn't support video playback.
		</video>
		<div
			class="psite-main-message mx-auto"
			v-html="main_message">
		</div>
	</div>
</template>

<script>
	export default {
		name: 'psite-home',
		data() {
			return {
				video_source: '@/assets/video/background_blur.webm',
				main_message: "Don't Wait For Opportunity. <br/>Create It.",
			}
		},
		mounted() {
			this.$refs.psite_bg_vid.play()
		}
	}
</script>

<style lang="scss">
	.psite-home {
		width: 100%;
		height: 100%;

		.psite-video-background {
			position: absolute;
			right: 0;
			bottom: 0;
			top:0;
			right:0;
			width: 100%;
			height: 100%;
			background-size: 100% 100%;
	 		background-color: black;
	  		background-position: center center;
	  		background-size: contain;
	   		object-fit: cover;
	   		z-index: 2;
		}

		.psite-main-message {
			position: absolute;
			top: 40%;
			left: 26%;
			width: 48%;
			background: transparent;
			z-index: 3;
			font-size: 30pt;
			font-family: 'Arial Black', 'Avenir', 'Tahoma';
			color: #fff;
			font-variant: small-caps;
			font-weight: bolder;
			// border: 5px solid #fff;

		}
	}
</style>
