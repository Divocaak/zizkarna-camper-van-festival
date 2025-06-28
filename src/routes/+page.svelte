<script>
	import ContactRow from '$lib/ContactRow.svelte';
	import ContentBlock from '$lib/ContentBlock.svelte';
	import FormButton from '$lib/FormButton.svelte';
</script>

<div class="landing">
	<div class="content">
		<img src="/sticker.png" alt="landing sticker" />
		<FormButton />
	</div>
</div>

<ContentBlock title="O festivalu">
	<div slot="left">
		<p>left</p>
	</div>
	<div slot="right">
		<p>right</p>
	</div>
</ContentBlock>

<ContentBlock title="O Žižkárně">
	<div slot="left">
		<p>left</p>
	</div>
	<div slot="right" class="about-img-wrapper">
		<img src="/about/0.jpg" alt="about zizkarna" />
		<img src="/about/1.jpg" alt="about zizkarna" />
		<img src="/about/2.jpg" alt="about zizkarna" />
		<img src="/about/3.jpg" alt="about zizkarna" />
	</div>
</ContentBlock>

<ContentBlock title="Aktivity">
	<div slot="left">
		<p>left</p>
	</div>
	<div slot="right" class="button-wrapper">
		<FormButton />
	</div>
</ContentBlock>

<ContentBlock title="Kontakty">
	<div slot="left">
		<iframe
			src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2915.705759358011!2d14.48279907659605!3d48.97214539269423!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47734f8fb6d689ab%3A0x30873f0fb4b41a4c!2zxb1pxb5rw6FybmE!5e1!3m2!1scs!2scz!4v1740487550291!5m2!1scs!2scz"
			title="map"
			width="100%"
			height="100%"
			style="border:0; box-sizing: border-box;"
			allowfullscreen=""
			loading="lazy"
			referrerpolicy="no-referrer-when-downgrade"
		></iframe>
	</div>
	<div slot="right" class="contacts-wrapper">
		<ContactRow label="tst" mail="camperfest@zizkarna.cz" />
		<ContactRow label="tst" mail="technika@zizkarna.cz" />
		<ContactRow label="tst" mail="media@zizkarna.cz" />
	</div>
</ContentBlock>

<!-- TODO signature -->
<!-- TODO delete /ref.pdf -->
<!-- TODO seo jsons -->
<!-- TOGO ganal -->

<style>
	.landing {
		position: relative;
		width: 100%;
		height: 100vh;

		background-image: url('/landing.jpg');
		background-position: center;
		background-repeat: none;
		background-size: cover;
	}

	.landing .content {
		width: 100%;
		height: 100%;

		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.landing .content img {
		width: 35%;
		height: auto;
	}

	.about-img-wrapper {
		display: grid;
		grid-template-columns: 1fr 1fr;
		grid-template-rows: 1fr 1fr;
	}

	.about-img-wrapper img {
		width: calc(100% - var(--general-padding) / 2);
		height: auto;
		justify-self: center;
		padding: calc(var(--general-padding) / 4);
	}

	.button-wrapper {
		position: relative;
		display: flex;
	}

    .contacts-wrapper{
        display: flex;
        flex-direction: column;
    }
</style>
