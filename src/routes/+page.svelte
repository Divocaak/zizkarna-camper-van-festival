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
			"@type": "MusicFestival",
			"name": "DIY Caravan Festival 2025",
			"description": {
				"cs": "🚙 Nomádi přijíždějí do Budějc! 🛠️ Přehlídka karavanů, přívěsů, pick-upů a mnoho dalšího ve stylu udělej si sám (DIY). 🎸 Těšit se také můžete na workshopy, přednášky a koncerty.",
				"en": "🚙 Nomads are coming to Budějce! 🛠️ A showcase of caravans, trailers, pick-ups, and much more in a DIY (do-it-yourself) style. 🎸 You can also look forward to workshops, talks, and concerts.",
				"de": "🚙 Nomaden kommen nach Budějce! 🛠️ Eine Ausstellung von Wohnwagen, Anhängern, Pick-ups und vielem mehr im DIY-(Do-it-yourself)-Stil. 🎸 Freut euch außerdem auf Workshops, Vorträge und Konzerte."
			},
			"startDate": "2025-09-26",
			"endDate": "2025-09-27",
			"eventStatus": "https://schema.org/EventScheduled",
			"eventAttendanceMode": "https://schema.org/OfflineEventAttendanceMode",
			"image": "https://program.zizkarna.cz/dynamic/events/277.jpg",
			"url": "https://program.zizkarna.cz/",
			"keywords": ["festival", "hudba", "workshop", "karavany", "přednášky", "koncerty"],
			"location": {
				"@type": "MusicVenue",
				"name": "Žižkárna",
				"address": {
					"@type": "PostalAddress",
					"streetAddress": "Žižkova tř. 171/28",
					"addressLocality": "České Budějovice 6",
					"addressRegion": "České Budějovice",
					"postalCode": "37004",
					"addressCountry": "CZ"
				},
				"sameAs": [
					"https://zizkarna.cz/",
					"https://program.zizkarna.cz/",
					"https://www.instagram.com/zizkarna",
					"https://www.facebook.com/zizkarnacb/",
					"https://www.youtube.com/@Zizkarna"
				]
			},
			"organizer": {
				"@type": "Organization",
				"name": "Žižkárna",
				"url": "https://zizkarna.cz",
				"contactPoint": {
					"@type": "ContactPoint",
					"email": "info@zizkarna.cz",
					"telephone": "+420722680481"
				}
			},
			"offers": {
				"@type": "Offer",
				"price": "0",
				"priceCurrency": "CZK",
				"availability": "https://schema.org/InStoreOnly",
				"url": "https://program.zizkarna.cz/"
			},
			"subEvent": [
				{
					"@type": "MusicEvent",
					"name": {
						"cs": "DIY Caravan Festival: pátek",
						"en": "DIY Caravan Festival: Friday",
						"de": "DIY Caravan Festival: Freitag"
					},
					"startDate": "2025-09-26",
					"endDate": "2025-09-26",
					"inLanguage": ["cs", "en", "de"],
					"description": {
						"cs": "🚙 Nomádi přijíždějí do Budějc! 🛠️ Přehlídka karavanů, přívěsů, pick-upů a mnoho dalšího ve stylu udělej si sám (DIY). 🎸 Těšit se také můžete na workshopy, přednášky a koncerty.",
						"en": "🚙 Nomads are coming to Budějce! 🛠️ A showcase of caravans, trailers, pick-ups, and much more in a DIY style. 🎸 You can also look forward to workshops, talks, and concerts.",
						"de": "🚙 Nomaden kommen nach Budějce! 🛠️ Eine Ausstellung von Wohnwagen, Anhängern, Pick-ups und vielem mehr im DIY-Stil. 🎸 Freut euch außerdem auf Workshops, Vorträge und Konzerte."
					},
					"doorTime": "15:00:00",
					"url": "https://program.zizkarna.cz/277",
					"image": "https://program.zizkarna.cz/dynamic/events/277.jpg",
					"isAccessibleForFree": true,
					"eventAttendanceMode": "https://schema.org/OfflineEventAttendanceMode",
					"eventStatus": "https://schema.org/EventScheduled",
					"location": {
						"@type": "MusicVenue",
						"name": "Žižkárna",
						"address": {
							"@type": "PostalAddress",
							"streetAddress": "Žižkova tř. 171/28",
							"addressLocality": "České Budějovice 6",
							"addressRegion": "České Budějovice",
							"postalCode": "37004",
							"addressCountry": "CZ"
						},
						"sameAs": [
							"https://zizkarna.cz/",
							"https://program.zizkarna.cz/",
							"https://www.instagram.com/zizkarna",
							"https://www.facebook.com/zizkarnacb/",
							"https://www.youtube.com/@Zizkarna"
						]
					},
					"performer": [
						{
							"@type": "MusicGroup",
							"name": "Nixon Lads",
							"performTime": "17:45:00",
							"genre": ["punk", "alternative", "indie"],
							"description": {
								"cs": "Nejlepší americká kapela ve Strakonicích se žánrově pohybuje někde na ose indie-alternative-punk se silným příklonem k devadesátkám.",
								"en": "An indie-alternative-punk band from Strakonice inspired by 90s sounds.",
								"de": "Eine Indie-Alternative-Punk-Band aus Strakonice, inspiriert von den 90er Jahren."
							},
							"sameAs": [
								"https://facebook.com/nixonlads",
								"https://instagram.com/nixonlads",
								"https://open.spotify.com/artist/2adwR18rLlxd9kr43jMUWt?si=292cf8b737264347"
							]
						},
						{
							"@type": "MusicGroup",
							"name": "Forest Ray",
							"performTime": "19:30:00",
							"genre": ["pop-rock", "folk", "psychedelický rock", "western"],
							"description": {
								"cs": "Psych-folk-rocková kapela Forest Ray vznikla v roce 2015 a spojuje prvky psych rocku s garážovým a folk rockem.",
								"en": "Forest Ray blends psychedelic folk-rock with garage and pop-rock influences since 2015.",
								"de": "Forest Ray kombiniert seit 2015 Psychedelic-Folk-Rock mit Garage- und Pop-Rock-Einflüssen."
							},
							"sameAs": [
								"https://open.spotify.com/artist/6aHS1ijoQqNunPy8K2zzAp",
								"https://instagram.com/forestrayrecords",
								"https://forestray.bandcamp.com/"
							]
						},
						{
							"@type": "MusicGroup",
							"name": "DJ Antonín Padrta",
							"performTime": "20:30:00",
							"genre": ["disco", "house", "funk", "soul"],
							"description": {
								"cs": "DJ z Českých Budějovic, který rozdává radost house music mixy s příměsí disco, funky a soulu.",
								"en": "A DJ from České Budějovice mixing house, disco, funk, and soul.",
								"de": "Ein DJ aus České Budějovice, der House, Disco, Funk und Soul mischt."
							},
							"sameAs": [
								"https://soundcloud.com/anton-n-padrta",
								"https://facebook.com/antonin.padrta/"
							]
						}
					]
				},
				{
					"@type": "MusicEvent",
					"name": {
						"cs": "DIY Caravan Festival: sobota",
						"en": "DIY Caravan Festival: Saturday",
						"de": "DIY Caravan Festival: Samstag"
					},
					"startDate": "2025-09-27",
					"endDate": "2025-09-27",
					"inLanguage": ["cs", "en", "de"],
					"description": {
						"cs": "🚙 Nomádi přijíždějí do Budějc! 🛠️ Přehlídka karavanů, přívěsů, pick-upů a mnoho dalšího ve stylu udělej si sám (DIY). 🎸 Těšit se také můžete na workshopy, přednášky a koncerty.",
						"en": "🚙 Nomads are coming to Budějce! 🛠️ A showcase of caravans, trailers, pick-ups, and much more in a DIY style. 🎸 You can also look forward to workshops, talks, and concerts.",
						"de": "🚙 Nomaden kommen nach Budějce! 🛠️ Eine Ausstellung von Wohnwagen, Anhängern, Pick-ups und vielem mehr im DIY-Stil. 🎸 Freut euch außerdem auf Workshops, Vorträge und Konzerte."
					},
					"doorTime": "15:00:00",
					"url": "https://program.zizkarna.cz/278",
					"image": "https://program.zizkarna.cz/dynamic/events/278.jpg",
					"isAccessibleForFree": true,
					"eventAttendanceMode": "https://schema.org/OfflineEventAttendanceMode",
					"eventStatus": "https://schema.org/EventScheduled",
					"location": {
						"@type": "MusicVenue",
						"name": "Žižkárna",
						"address": {
							"@type": "PostalAddress",
							"streetAddress": "Žižkova tř. 171/28",
							"addressLocality": "České Budějovice 6",
							"addressRegion": "České Budějovice",
							"postalCode": "37004",
							"addressCountry": "CZ"
						},
						"sameAs": [
							"https://zizkarna.cz/",
							"https://program.zizkarna.cz/",
							"https://www.instagram.com/zizkarna",
							"https://www.facebook.com/zizkarnacb/",
							"https://www.youtube.com/@Zizkarna"
						]
					},
					"performer": [
						{
							"@type": "MusicGroup",
							"name": "Strejda Erdja",
							"performTime": "16:30:00",
							"genre": ["hip hop", "street dance"],
							"description": {
								"cs": "Energický hip-hopový performer, který propojuje hudbu a street dance.",
								"en": "Energetic hip-hop performer combining music and street dance.",
								"de": "Energiegeladener Hip-Hop-Künstler, der Musik und Street Dance verbindet."
							},
							"sameAs": [
								"https://instagram.com/strejda_erdja/",
								"https://facebook.com/profile.php?id=100079653230239"
							]
						},
						{
							"@type": "MusicGroup",
							"name": "Pobodá",
							"performTime": "19:00:00",
							"genre": ["bigbeat"],
							"description": {
								"cs": "Poctivej západočeskej skejtovej bigbeat. Šestičlené uskupení, jehož vystoupení tě pohladí po duši a pobodá do uší.",
								"en": "Authentic West Bohemian skate bigbeat with an emotional punch.",
								"de": "Authentischer westböhmischer Skate-Bigbeat mit emotionaler Power."
							},
							"sameAs": ["https://youtube.com/watch?v=VuLcCICWdk4", "https://instagram.com/_poboda"]
						},
						{
							"@type": "MusicGroup",
							"name": "Stepní běžec",
							"performTime": "20:30:00",
							"genre": ["post", "acid", "western"],
							"description": {
								"cs": "Čtyřčlenný dostavník z Prahy vezoucí westernové kytary vyprahlou krajinou.",
								"en": "A four-member Prague band riding through dusty landscapes with western guitars.",
								"de": "Vierköpfige Band aus Prag, die mit Western-Gitarren durch staubige Landschaften fährt."
							},
							"sameAs": ["https://instagram.com/stepni_bezec_", "https://stepnibezec.bandcamp.com/"]
						}
					]
				}
			]
		}
	</script>
</svelte:head>

<div class="localization-btns-wrapper">
	<LocalizationButton label="cz" newVal="cs" />
	<LocalizationButton label="en" newVal="en" />
	<LocalizationButton label="de" newVal="de" />
</div>

<div class="landing">
	<div class="content">
		<img src="/sticker.png" alt="landing sticker" />
		<FormButton />
	</div>
</div>

<ContentBlock title={langs[$lang].about.label} icon="car.svg">
	<div slot="left" class="button-wrapper"><FormButton /></div>
	<div slot="right"><p>{langs[$lang].about.text}</p></div>
</ContentBlock>

<ContentBlock title={langs[$lang].zizkarna.label} icon="character.svg" imgGal={true}>
	<div slot="left"><p>{langs[$lang].zizkarna.text}</p></div>
	<div slot="right" class="about-img-wrapper">
		<img src="/about/0.jpg" alt="about zizkarna" />
		<img src="/about/1.jpg" alt="about zizkarna" />
		<img src="/about/2.jpg" alt="about zizkarna" />
		<img src="/about/3.jpg" alt="about zizkarna" />
	</div>
</ContentBlock>

<ContentBlock title={langs[$lang].programme.label} icon="fire.svg">
	<div slot="left">
		{#each langs[$lang].programme.texts as text}<p>{text}</p>{/each}
	</div>
	<div slot="right" class="button-wrapper"><FormButton /></div>
	<div slot="left-bottom">
		<h2>
			<a href="https://program.zizkarna.cz/277" target="_blank">{langs[$lang].programme.friday}</a>
		</h2>
		<p>15:00 {langs[$lang].programme.doors}</p>
		<p>17:45 Nixon Lads</p>
		<p>19:30 Forest Ray</p>
		<p>20:30 DJ Antonín Padrta</p>
	</div>
	<div slot="right-bottom">
		<h2>
			<a href="https://program.zizkarna.cz/278" target="_blank">{langs[$lang].programme.saturday}</a
			>
		</h2>
		<p>15:00 {langs[$lang].programme.doors}</p>
		<p>16:30 Strejda Erdja</p>
		<p>19:00 Pobodá</p>
		<p>20:30 Stepní běžec</p>
	</div>
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
		<p class="signature">
			Coded and maintained by <a href="https://divokyvojtech.cz" target="_blank">Vojtěch Divoký</a>
		</p>
	</div>
</ContentBlock>

<style>
	.localization-btns-wrapper {
		display: flex;
		position: fixed;
		z-index: 100;
		width: calc(100% - 2 * 0.5rem);
		justify-content: end;
		gap: 0.5rem;
		padding: 0.5rem;
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
		width: calc(100% - var(--general-padding) / 8);
		height: auto;
		justify-self: center;
		padding: calc(var(--general-padding) / 8);
	}

	.button-wrapper {
		position: relative;
		display: flex;
		height: 100%;
		flex-direction: column;
		align-items: center;
		justify-content: center;
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

	.signature,
	.signature a {
		padding-top: 200px;
		font-size: var(--fs-8);
		text-align: end;
	}

	h2:has(> a) {
		text-align: center;
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
