<template>
	<div class="psite">
		<div class="psite-header">
			<app-header/>
		</div>
		<!-- <full-page
			ref="fullpage"
			:skip-init="true"
			:options="fp_options">
			<div class="section"> -->
				<app-home
					/>
			<!-- </div> -->
			<!-- <div class="section"> -->
				<app-about/>
			<!-- </div> -->
			<!-- <div class="section"> -->
				<app-resume/>
			<!-- </div> -->
			<!-- <div class="section"> -->
				<app-gbuilds/>
			<!-- </div> -->
			<!-- <div class="section"> -->
				<app-contact/>
			<!-- </div> -->
		<!-- </full-page> -->
	</div>
</template>

<script>
	import AppHeader from './AppHeader.vue'
	import AppHome from './AppHome.vue'
	import AppAbout from './AppAbout.vue'
	import AppResume from './AppResume.vue'
	import AppGbuilds from './AppGbuilds.vue'
	import AppContact from './AppContact.vue'

	export default {
		name: 'app-main',
		components: {
			AppHeader,
			AppHome,
			AppAbout,
			AppResume,
			AppGbuilds,
			AppContact
		},
		data() {
			return {
				fp_options: {
					licenseKey: 'GPLv3',
			        menu: '#psite-header',
			        anchors: ['psite-home', 'psite-about', 'psite-resume', 'psite-gbuilds', 'psite-contact'],
				},
				fp_ref: {}
			}
		},

		mounted() {
			this.fp_ref = this.$refs.fullpage
			this.$refs.fullpage.init()
			window.ps = this
		}
	}
</script>
<style lang="scss">
	.psite {
		.psite-body {
			display: block;
		}
	}
</style>
