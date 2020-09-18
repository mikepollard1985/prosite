<template>
	<div
		class="psite-header"
		id="psite-header">
		<div class="row">
			<div class="col-sm-2 header-image mr-auto">
				<a href="#psite-home">
					<img src="@/assets/img/logo_transparent.png" width="78" height="100" />
				</a>
			</div>
			<div class="col-sm-3 header-buffer"></div>
			<div
				class="col-sm-7 psite-navbar">
				<nav class="navbar navbar-right navbar-expand-lg navbar-light bg-transparent ml-auto">
					<button class="navbar-toggler ml-auto" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
						<span class="navbar-toggler-icon"></span>
					</button>
					<div class="collapse navbar-collapse" id="navbarNav">
						<ul class="navbar-nav ml-auto">
							<li class="nav-item active">
								<a class="nav-link" href="#psite-home">HOME <span class="sr-only">(current)</span></a>
							</li>
							<li class="nav-item">
								<a class="nav-link" href="#psite-about">ABOUT </a>
							</li>
							<li class="nav-item">
								<a class="nav-link" href="#psite-resume">RESUME </a>
							</li>
							<li class="nav-item">
								<a class="nav-link" href="#psite-gbuilds">GAMING/BUILDS </a>
							</li>
							<li class="nav-item">
								<a class="nav-link" href="#psite-contact">CONTACT </a>
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
			return {}
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
		text-align: right;
		width: 100%;
		z-index: 5;
		color: black;

		.psite-navbar {
			color: black;
			padding-top: 15px;
			text-align: right;
			font-size: 15pt;
			font-weight: 500;
		}

		.header-image {
			text-alight: left !important;
		}
	}
</style>
