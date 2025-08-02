<script>
	export let label;
	export let mail;
</script>

<p>{@html label}:</p>
<a href="mailto:{mail}">{mail}</a>

<style>
	@media only screen and (max-width: 600px) {
		p,
		a {
			font-size: var(--fs-20);
		}
	}
</style>
