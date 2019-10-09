<script>
	import HeadingHero from './heading-hero.svelte';
	import SubHeadingHero from './subheading-hero.svelte';
	import Button from './button.svelte';
	import Content from './content.svelte';

	export let heading;
	export let subheading;
	export let actions = [];
	export let overlay = false;
</script>

<style>
	.hero {
		position: relative;
		background-image: url(../images/intro-bg.jpg);
		background-attachment: fixed;
		background-repeat: no-repeat;
		background-position: center top;
		background-size: cover;
		text-align: center;
		padding-top: 15.6rem;
		overflow: hidden;
	}
	.actions {
		margin-bottom: 4.2rem;
	}
	:global(.hero img) {
		vertical-align: bottom;
		max-width: 840px;
		width: 100%;
		box-shadow: 0 -1px 5px rgba(0, 0, 0, 0.3);
	}
	.shadow-overlay {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		opacity: 0.5;
		background: linear-gradient(
			to bottom,
			transparent 0%,
			rgba(0, 0, 0, 0.8) 100%
		);
		filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#00000000', endColorstr='#cc000000', GradientType=0);
	}

	/* ------------------------------------------------------------------- 
 * responsive:
 * intro
 * ------------------------------------------------------------------- */
	@media only screen and (max-width: 1024px) {
		.hero {
			padding-top: 15rem;
		}

		:global(.hero h1) {
			font-size: 5rem;
			padding: 0 6%;
		}
	}
	@media only screen and (max-width: 768px) {
		.hero {
			padding-top: 13.8rem;
		}

		:global(.hero h3) {
			font-size: 1.8rem;
			letter-spacing: 0.4rem;
		}

		:global(.hero h1) {
			font-size: 4.5rem;
			padding: 0;
		}
	}
	@media only screen and (max-width: 600px) {
		.hero {
			padding-top: 13.2rem;
		}

		:global(.hero h3) {
			font-size: 1.7rem;
			letter-spacing: 0.35rem;
		}

		:global(.hero h1) {
			font-size: 4rem;
			padding: 0;
		}
	}
	@media only screen and (max-width: 500px) {
		.hero {
			padding-top: 12rem;
		}

		:global(.hero h3) {
			font-size: 1.6rem;
			letter-spacing: 0.3rem;
		}

		:global(.hero h1) {
			font-size: 3.8rem;
			padding: 0;
		}

		.hero .actions {
			max-width: 320px;
			width: 100%;
			margin-left: auto;
			margin-right: auto;
		}

		:global(.hero .actions .button) {
			display: block;
			width: 100%;
			margin: 0 0 1.5rem 0;
		}
	}
	@media only screen and (max-width: 400px) {
		:global(.hero h3) {
			font-size: 1.5rem;
			letter-spacing: 0.3rem;
		}

		:global(.hero h1) {
			font-size: 3.5rem;
			padding: 0;
		}

		.hero .actions {
			width: 100%;
		}
	}
</style>

<section class="hero">
	<Content>
		{#if overlay}
			<div class="shadow-overlay" />
		{/if}
		{#if subheading}
			<SubHeadingHero>{subheading}</SubHeadingHero>
		{/if}
		{#if heading}
			<HeadingHero>{heading}</HeadingHero>
		{/if}
		{#if actions}
			<div class="actions">
				{#each actions as { label, href, onClick }, i}
					<Button invert {href} {onClick}>{label}</Button>
				{/each}
			</div>
		{/if}
		<slot />

	</Content>
</section>
