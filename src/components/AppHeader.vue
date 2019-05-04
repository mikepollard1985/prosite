<template>
	<div
		class="psite-header"
		id="psite-header">
		<div class="row">
			<div class="col-2 header-image">
				<img src="../assets/img/logo_transparent.png" width="78" height="100" />
			</div>
			<div class="col-5 header-buffer"></div>
			<div
				class="col-5 psite-navbar">
				<nav class="navbar navbar-expand-lg navbar-light bg-transparent ml-auto">
					<button class="navbar-toggler ml-auto" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
						<span class="navbar-toggler-icon"></span>
					</button>
					<div class="collapse navbar-collapse" id="navbarNav">
						<ul class="navbar-nav">
							<li class="nav-item active">
								<a class="nav-link" href="#">HOME <span class="sr-only">(current)</span></a>
							</li>
							<li class="nav-item">
								<a class="nav-link" href="#">ABOUT </a>
							</li>
							<li class="nav-item">
								<a class="nav-link" href="#">RESUME </a>
							</li>
							<li class="nav-item">
								<a class="nav-link" href="#">GAMING/BUILDS </a>
							</li>
							<li class="nav-item">
								<a class="nav-link" href="#">CONTACT </a>
							</li>
						</ul>
					</div>
				</nav>
			</div>
		</div>
	</div>
</template>

<script>
	export default {
		name: 'app-header',
		data() {
			return {
			}
		}
	}
</script>

<style lang="scss">
	.psite-header {
		background: transparent;
		margin: 0px;
		padding: 10px 20px;
		position: fixed;
		top: 0px;
		width: 100%;

		.psite-navbar {
			padding-top: 15px;
			text-align: right;
		}
	}
</style>
