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
			<Logo width="150" height="150" />
		</div>
		<div class="main-info">
			<h1>Hello {name}!</h1>
			<PageText />
		</div>
		<div class="side-block">
		</div>
	</div>
</main>

<style>
	main {
		text-align: center;
		max-width: 240px;
		height: 100%;
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
		justify-content: flex-start;
		height: 100%;
	}

	.main-info {
		max-width: 1200px;
		text-align: left;
		margin: 0 auto;
		padding: 24px;
	}

	.side-block {
		height: 100%;
		min-width: 100px;
		max-width: 500px;
		background-color: lightblue;
	}

	.header {
		height: 80px;
		max-height: 80px;
		width: 100%;
		padding-left: 8px;
		text-align: left;
		background-color: lightblue;
		display: grid;
	}
</style>