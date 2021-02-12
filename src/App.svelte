<script>
	import Logo from './assets/images/equus-logo.svg';
	import PageText from './assets/posts/front-page.md';
	export let name;
</script>

<main>
	<div class="header">
		<Logo width="80" height="80" />
	</div>
	<div class="main-body">
		<div class="side-block">
			<Logo width="300" height="300" />
		</div>
		<div class="main-info">
			<h1>Hello {name}!</h1>
			<PageText />
		</div>
		<div class="side-block">
			<Logo width="300" height="300" />
		</div>
	</div>
</main>

<style>
	main {
		text-align: center;
		max-width: 240px;
	}

	h1 {
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}

	@media (max-width: 640px) {
		.side-block {
			display: none;
		}
	}

	.main-body {
		display: flex;
		flex-direction: row;
	}

	.main-info {
		max-width: 1200px;
		text-align: left;
		margin: auto;
		padding: 24px;
	}

	.side-block {
		min-width: 300px;
		max-width: 500px;
		background-color: blueviolet;
	}

	.header {
		height: 80px;
		max-height: 80px;
		width: 100%;
		padding-left: 8px;
		text-align: left;
		background-color: blueviolet;
		display: grid;
	}
</style>