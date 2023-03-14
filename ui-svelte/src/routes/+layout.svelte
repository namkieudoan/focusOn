<script>
	import Header from './Header.svelte';
	import './styles.css';
</script>

<div class="app">
	<Header/>
	<main class="main">
		<slot />
	</main>
</div>
	
<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;

	}
	.main {
		max-width: 680px;
		margin: auto;
	}
	@media (max-width: 480px) {
		.app {
			padding:0 12px;
		}
	}
</style>
