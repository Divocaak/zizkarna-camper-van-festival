<script>
	import { lang } from '$lib/stores/LangStore.js';
	export let label;
	export let newVal;
</script>

<button onclick={() => lang.set(newVal)}>{label}</button>

<style>
	button {
		position: relative;
		background-color: var(--grey);
		color: var(--light-grey);
		border: 2px solid var(--grey);

		padding: calc(var(--general-padding) / 5);
		border-radius: 1rem;

		/* margin: 1rem; */

		text-transform: uppercase;

		transition: all 0.25s ease-in-out;
	}

	button:hover {
		background-color: var(--light-grey);
		color: var(--purple);
		border: 2px solid var(--purple);
	}
</style>
