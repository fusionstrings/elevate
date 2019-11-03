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
<section id={id} class="features">
	<Content>
		<slot name="section-lead" />
		<slot />
	</Content>
</section>
<!-- /features -->
