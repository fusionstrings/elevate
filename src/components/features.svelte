<script>
	import Lead from './lead.svelte';
	import SectionLead from './section-lead.svelte';
	import FeatureBlock from './feature-block.svelte';
	import Content from './content.svelte';
	export let id = '';
</script>

<style>
	/* ===================================================================
 * 12. features - (_layout.scss)
 *
 * ------------------------------------------------------------------- */
	.features {
		padding: 15rem 0 12rem;
		background-color: var(--brand-color);
		overflow: hidden;
	}
	:global(.features h1, .features h2, .features h3, .features h4, .features
			h5, .features h6, .features .h01, .features .h02, .features
			.h03, .features .h04, .features .h05, .features .h06) {
		color: var(--text-color-heading);
	}

	/* ------------------------------------------------------------------- 
 * responsive:
 * features
 * ------------------------------------------------------------------- */
	@media only screen and (max-width: 768px) {
		.features {
			padding: 11.4rem 0 10.6rem;
		}
	}
</style>

<!-- features
   	================================================== -->
<section {id} class="features">
	<Content>
		<slot name="section-lead" />
		<slot />
	</Content>
</section>
<!-- /features -->
