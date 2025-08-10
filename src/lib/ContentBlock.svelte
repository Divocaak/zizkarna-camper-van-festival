<script>
	export let title;
	export let icon;

	export let imgGal = false;
</script>

<div class="wrapper">
	<img src="/icons/{icon}" alt="svg icon" />
	<h1>{@html title}</h1>
	<div class="content-wrapper">
		<div class="left" class:img-gal={imgGal}><slot name="left"></slot></div>
		<div class="right" class:img-gal={imgGal}><slot name="right"></slot></div>
	</div>
</div>

<style>
	.wrapper {
		width: 100%;
		min-height: 100vh;
		background-color: var(--light-grey);
	}

	.wrapper h1 {
		width: calc(100% - 2 * var(--general-padding));
		border-bottom: 2px solid var(--yellow);

		padding: var(--general-padding);
		padding-bottom: 0;
	}

	.wrapper img {
		height: 90px;
		width: auto;
		position: absolute;
		left: 50%;
		transform: translateX(-50%);
	}

	.content-wrapper {
		height: 100%;
		width: calc(100% - 2 * var(--general-padding));

		display: flex;
		flex-direction: row;

		padding: var(--general-padding);
		padding-top: 0;
	}

	.content-wrapper .left,
	.content-wrapper .right {
		width: 50%;
		min-height: 100%;

		display: flex;
		flex-direction: column;

		align-items: stretch;
		justify-content: flex-start;
	}

	
	.content-wrapper .left {
		margin-right: var(--general-padding);
	}
	
	.content-wrapper .right {
		margin-left: var(--general-padding);
	}

	.content-wrapper .left.img-gal{
		width: 45%;
	}

	.content-wrapper .right.img-gal{
		margin-left: 0;
		width: 55%;

		align-items: center;
		justify-content: center;
	}

	@media only screen and (max-width: 600px) {
		.wrapper h1 {
			padding: calc(var(--general-padding) / 5);
			width: calc(100% - 2 * (var(--general-padding) / 5));
			padding-top: 150px;
			text-align: center;
			font-size: var(--fs-44);
		}

		.content-wrapper {
			flex-direction: column;
			padding: calc(var(--general-padding) / 4);
			width: calc(100% - 2 * (var(--general-padding) / 4));
		}

		.content-wrapper .left,
		.content-wrapper .right,
		.content-wrapper .left.img-gal,
		.content-wrapper .right.img-gal {
			margin: 0;
			width: 100%;
		}
	}
</style>
