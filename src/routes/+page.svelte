<script>
	import { lang } from '$lib/stores/LangStore.js';
	import langs from '$lib/localization.json';

	import ContactRow from '$lib/ContactRow.svelte';
	import ContentBlock from '$lib/ContentBlock.svelte';
	import FormButton from '$lib/FormButton.svelte';
	import LocalizationButton from '$lib/LocalizationButton.svelte';
</script>

<svelte:head>
	<script type="application/ld+json">
		{
			"@context": "https://schema.org",
			"@type": "Festival",
			"name": "DHOGH Festival 2025",
			"startDate": "2025-06-18",
			"endDate": "2025-06-20",
			"location": {
				"@type": "Place",
				"name": "Žižkárna",
				"url": "https://zizkarna.cz",
				"address": {
					"@type": "PostalAddress",
					"streetAddress": "Žižkova tř. 28",
					"addressLocality": "České Budějovice",
					"addressCountry": "CZ"
				}
			},
			"description": "Festival propojuje taneční hudbu, umění, filozofii a komunitního ducha undergroundové scény. Poskytuje nejen kulturní zážitek, ale i prostor pro hlubší reflexi nad významem elektronické hudby a jejího vlivu na městský noční život."
		}
	</script>
</svelte:head>

<div class="localization-btns-wrapper">
	<LocalizationButton label="cz" newVal="cs" />
	<LocalizationButton label="en" newVal="en" />
</div>

<div class="landing">
	<div class="content">
		<img src="/sticker.png" alt="landing sticker" />
		<FormButton />
	</div>
</div>

<ContentBlock title={langs[$lang].about.label} icon="car.svg">
	<div slot="left"><p>{langs[$lang].about.left}</p></div>
	<div slot="right"><p>{langs[$lang].about.right}</p></div>
</ContentBlock>

<ContentBlock title={langs[$lang].zizkarna.label} icon="character.svg">
	<div slot="left"><p>{langs[$lang].zizkarna.text}</p></div>
	<div slot="right" class="about-img-wrapper">
		<img src="/about/0.jpg" alt="about zizkarna" />
		<img src="/about/1.jpg" alt="about zizkarna" />
		<img src="/about/2.jpg" alt="about zizkarna" />
		<img src="/about/3.jpg" alt="about zizkarna" />
	</div>
</ContentBlock>

<ContentBlock title={langs[$lang].activities.label} icon="fire.svg">
	<div slot="left"><p>{langs[$lang].activities.text}</p></div>
	<div slot="right" class="button-wrapper"><FormButton /></div>
</ContentBlock>

<ContentBlock title={langs[$lang].contacts.label} icon="car.svg">
	<div slot="left">
		<iframe
			src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2915.705759358011!2d14.48279907659605!3d48.97214539269423!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47734f8fb6d689ab%3A0x30873f0fb4b41a4c!2zxb1pxb5rw6FybmE!5e1!3m2!1scs!2scz!4v1740487550291!5m2!1scs!2scz"
			title="map"
			class="contacts-map"
			allowfullscreen
			loading="lazy"
			referrerpolicy="no-referrer-when-downgrade"
		></iframe>
	</div>
	<div slot="right" class="contacts-wrapper">
		<ContactRow label={langs[$lang].contacts.organizational} mail="camperfest@zizkarna.cz" />
		<ContactRow label={langs[$lang].contacts.technical} mail="technika@zizkarna.cz" />
		<ContactRow label={langs[$lang].contacts.media} mail="media@zizkarna.cz" />
		<p class="signature">Coded and maintained by <a href="https://divokyvojtech.cz" target="_blank">Vojtěch Divoký</a></p>
	</div>
</ContentBlock>

<!-- TODO meta tags RADEK -->
<!-- TODO seo jsons -->

<style>
	.localization-btns-wrapper{
		display: flex;
		position: fixed;
		z-index: 100;
		width: calc(100% - 2* .5rem);
		justify-content: end;
		gap: .5rem;
		padding: .5rem;
	}

	.landing {
		position: relative;
		width: 100%;
		height: 100vh;

		background-image: url('/landing.jpg');
		background-position: center;
		background-repeat: none;
		background-size: cover;
		background-attachment: fixed;
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

	.contacts-wrapper {
		display: flex;
		flex-direction: column;
	}

	.contacts-map {
		border: 0;
		box-sizing: border-box;
		width: 100%;
		height: 400px;
	}

	.signature, .signature a{
		padding-top: 200px;
		font-size: var(--fs-8);
		text-align: end;
	}

	@media only screen and (max-width: 600px) {
		.landing .content img {
			width: 92%;
		}

		.about-img-wrapper {
			grid-template-columns: 1fr;
			grid-template-rows: repeat(4, 1fr);
		}

		.about-img-wrapper img {
			width: calc(100% - var(--general-padding) / 8);
			padding: calc(var(--general-padding) / 16);
		}

		.contacts-map {
			width: 100%;
		}
	}
</style>
