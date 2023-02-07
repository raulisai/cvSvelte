<script>
	import Header from './Header.svelte';
	import './styles.css';
</script>

<div class="app">
	<Header />

	<main class="container-fluid">
		<slot />
	</main>

	<footer>
		<p>visit <a href="https://raulisai.github.io/">raulisai.github.io/</a> my cv</p>
	</footer>
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	main {
		
	}

	footer {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 12px;
	}

	footer a {
		font-weight: bold;
	}

	@media (min-width: 480px) {
		footer {
			padding: 12px 0;
		}
	}
</style>
