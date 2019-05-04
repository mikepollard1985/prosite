<template>
	<div id="app">
		<app-main></app-main>
	</div>
</template>

<script>
import AppMain from './components/AppMain.vue'

export default {
	name: 'app',
	components: {
		AppMain
	}
}
</script>

<style lang="scss">
	#app {
		font-family: 'Avenir', Helvetica, Arial, sans-serif;
		-webkit-font-smoothing: antialiased;
		-moz-osx-font-smoothing: grayscale;
		text-align: center;
		color: #2c3e50;
		& a {
			color: #fff;
		}

	}
</style>
