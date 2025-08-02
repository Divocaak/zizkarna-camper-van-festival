<script>
	import { lang } from '$lib/stores/LangStore.js';
	import langs from '$lib/localization.json';
</script>

<a href="/">{@html langs[$lang].formButtonText}</a>

<style>
	a {
		position: relative;
		background-color: var(--grey);
		color: var(--light-grey);
		border: 2px solid var(--grey);

		padding: calc(var(--general-padding) / 3);
		border-radius: 1rem;

		margin: 1rem;
	}

	a:hover {
		background-color: var(--light-grey);
		color: var(--purple);
		border: 2px solid var(--purple);
	}
</style>
