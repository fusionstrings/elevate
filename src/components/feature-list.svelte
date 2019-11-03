<style>
	/* ===================================================================
 * 12. features - (_layout.scss)
 *
 * ------------------------------------------------------------------- */
	:global(.features .feature-list),
	.feature-list {
		margin-top: 1.5rem;
		display: grid;
		grid-template-columns: repeat(
			auto-fill,
			minmax(calc(var(--content-max-width) / 3), 1fr)
		);
	}
</style>

<div class="feature-list">
	<slot />
</div>
