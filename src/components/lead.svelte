<script>
	export let content;
</script>

<style>
	:global(p.lead) {
		font-weight: var(--font-weight-light);
		font-size: 2.1rem;
		line-height: 1.714;
		color: var(--text-color-lead);
	}

	@media only screen and (max-width: 768px) {
		:global(p.lead) {
			font-size: 1.9rem;
		}
	}
</style>

{#if content}
	<p class="lead">{content}</p>
{/if}

<p class="lead">
	<slot />
</p>
