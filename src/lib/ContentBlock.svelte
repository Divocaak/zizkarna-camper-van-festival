<script>
	export let title;
	export let icon;
</script>

<div class="wrapper">
	<h1>{title}</h1>
	<img src="/icons/{icon}" alt="svg icon"/>
    <!-- TODO icon -->
	<div class="content-wrapper">
		<div class="left"><slot name="left"></slot></div>
		<div class="right"><slot name="right"></slot></div>
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
        align-items: center;
        justify-content: center;
	}

    .content-wrapper .left{
        margin-right: var(--general-padding);
    }

    .content-wrapper .right{
        margin-left: var(--general-padding);
    }
</style>
