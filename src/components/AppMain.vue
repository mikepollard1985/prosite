<template>
	<div class="body">
		<app-header></app-header>
		<video autoplay muted loop class="psite-video-background">
			<source src="../assets/video/background-blur.mp4" type="video/mp4">
		</video>
	</div>
</template>

<script>
import AppHeader from './AppHeader.vue'
export default {
	name: 'app-main',
	components: {
		AppHeader
	},
	data() {
		return {
			video_source: '../assets/video/background-noblur.mp4'
		}
	}
}
</script>
u
<style lang="scss">
	.body {
		// background: #595959;
		.psite-video-background {
			width: 100%;
		}
	}
</style>
