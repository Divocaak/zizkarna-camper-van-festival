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

<ContentBlock title="O festivalu" icon="car.svg">
	<div slot="left">
		<p>
			Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Pellentesque habitant morbi
			tristique senectus et netus et malesuada fames ac turpis egestas. Duis pulvinar. In enim a
			arcu imperdiet malesuada. Nullam feugiat, turpis at pulvinar vulputate, erat libero tristique
			tellus, nec bibendum odio risus sit amet ante. Etiam sapien elit, consequat eget, tristique
			non, venenatis quis, ante. Proin pede metus, vulputate nec, fermentum fringilla, vehicula
			vitae, justo. Cras elementum. Nullam dapibus fermentum ipsum. Donec quis nibh at felis congue
			commodo. Etiam dui sem, fermentum vitae, sagittis id, malesuada in, quam. Nulla accumsan, elit
			sit amet varius semper, nulla mauris mollis quam, tempor suscipit diam nulla vel leo. Fusce
			nibh. Nullam rhoncus aliquam metus. Sed elit dui, pellentesque a, faucibus vel, interdum nec,
			diam. Integer imperdiet lectus quis justo. Etiam bibendum elit eget erat.
		</p>
	</div>
	<div slot="right">
		<p>
			Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Pellentesque habitant morbi
			tristique senectus et netus et malesuada fames ac turpis egestas. Duis pulvinar. In enim a
			arcu imperdiet malesuada. Nullam feugiat, turpis at pulvinar vulputate, erat libero tristique
			tellus, nec bibendum odio risus sit amet ante. Etiam sapien elit, consequat eget, tristique
			non, venenatis quis, ante. Proin pede metus, vulputate nec, fermentum fringilla, vehicula
			vitae, justo. Cras elementum. Nullam dapibus fermentum ipsum. Donec quis nibh at felis congue
			commodo. Etiam dui sem, fermentum vitae, sagittis id, malesuada in, quam. Nulla accumsan, elit
			sit amet varius semper, nulla mauris mollis quam, tempor suscipit diam nulla vel leo. Fusce
			nibh. Nullam rhoncus aliquam metus. Sed elit dui, pellentesque a, faucibus vel, interdum nec,
			diam. Integer imperdiet lectus quis justo. Etiam bibendum elit eget erat.
		</p>
	</div>
</ContentBlock>

<ContentBlock title="O Žižkárně" icon="character.svg">
	<div slot="left">
		<p>
			Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Pellentesque habitant morbi
			tristique senectus et netus et malesuada fames ac turpis egestas. Duis pulvinar. In enim a
			arcu imperdiet malesuada. Nullam feugiat, turpis at pulvinar vulputate, erat libero tristique
			tellus, nec bibendum odio risus sit amet ante. Etiam sapien elit, consequat eget, tristique
			non, venenatis quis, ante. Proin pede metus, vulputate nec, fermentum fringilla, vehicula
			vitae, justo. Cras elementum. Nullam dapibus fermentum ipsum. Donec quis nibh at felis congue
			commodo. Etiam dui sem, fermentum vitae, sagittis id, malesuada in, quam. Nulla accumsan, elit
			sit amet varius semper, nulla mauris mollis quam, tempor suscipit diam nulla vel leo. Fusce
			nibh. Nullam rhoncus aliquam metus. Sed elit dui, pellentesque a, faucibus vel, interdum nec,
			diam. Integer imperdiet lectus quis justo. Etiam bibendum elit eget erat.
		</p>
	</div>
	<div slot="right" class="about-img-wrapper">
		<img src="/about/0.jpg" alt="about zizkarna" />
		<img src="/about/1.jpg" alt="about zizkarna" />
		<img src="/about/2.jpg" alt="about zizkarna" />
		<img src="/about/3.jpg" alt="about zizkarna" />
	</div>
</ContentBlock>

<ContentBlock title="Aktivity" icon="fire.svg">
	<div slot="left">
		<p>
			Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Pellentesque habitant morbi
			tristique senectus et netus et malesuada fames ac turpis egestas. Duis pulvinar. In enim a
			arcu imperdiet malesuada. Nullam feugiat, turpis at pulvinar vulputate, erat libero tristique
			tellus, nec bibendum odio risus sit amet ante. Etiam sapien elit, consequat eget, tristique
			non, venenatis quis, ante. Proin pede metus, vulputate nec, fermentum fringilla, vehicula
			vitae, justo. Cras elementum. Nullam dapibus fermentum ipsum. Donec quis nibh at felis congue
			commodo. Etiam dui sem, fermentum vitae, sagittis id, malesuada in, quam. Nulla accumsan, elit
			sit amet varius semper, nulla mauris mollis quam, tempor suscipit diam nulla vel leo. Fusce
			nibh. Nullam rhoncus aliquam metus. Sed elit dui, pellentesque a, faucibus vel, interdum nec,
			diam. Integer imperdiet lectus quis justo. Etiam bibendum elit eget erat.
		</p>
	</div>
	<div slot="right" class="button-wrapper">
		<FormButton />
	</div>
</ContentBlock>

<ContentBlock title="Kontakty" icon="car.svg">
	<div slot="left">
        <div class="map-wrapper">

            <iframe
			src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2915.705759358011!2d14.48279907659605!3d48.97214539269423!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47734f8fb6d689ab%3A0x30873f0fb4b41a4c!2zxb1pxb5rw6FybmE!5e1!3m2!1scs!2scz!4v1740487550291!5m2!1scs!2scz"
			title="map"
			width="100%"
			height="100%"
			class="contacts-map"
			allowfullscreen=""
			loading="lazy"
			referrerpolicy="no-referrer-when-downgrade"
            ></iframe>
        </div>
	</div>
	<div slot="right" class="contacts-wrapper">
		<ContactRow label="tst" mail="camperfest@zizkarna.cz" />
		<ContactRow label="tst" mail="technika@zizkarna.cz" />
		<ContactRow label="tst" mail="media@zizkarna.cz" />
	</div>
</ContentBlock>

<!-- TODO icons on contentnt panels -->
<!-- TODO meta tags -->
<!-- TODO seo jsons -->
<!-- TODO ganal -->

<style>
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
        width: calc(100vw - 10*var(--general-padding));
        height: 300px;
	}
</style>
