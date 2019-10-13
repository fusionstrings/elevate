<script>
	export let order = '';
	export let title = '';
	export let content = '';
</script>

<style>
	:global(.features .feature-count),
	.feature-count {
		display: block;
		color: #ed254d;
		font-weight: var(--font-weight-bold);
		font-size: 4rem;
		line-height: 1;
		margin-bottom: 2.4rem;
	}
	:global(.features .feature),
	.feature {
		padding: 0 30px 1.5rem 30px;
	}
	:global(.features h3),
	h3 {
		font-weight: var(--font-weight-medium);
	}
	@media only screen and (max-width: 768px) {
		:global(.features .feature),
		.feature {
			padding: 0 15px;
		}
	}
    @media only screen and (max-width: 600px) {
		:global(.features .feature),
		.feature {
			padding: 0 10px;
		}
	}

	@media only screen and (max-width: 400px) {
		:global(.features .feature),
		.feature {
			padding: 0;
		}
	}
</style>

<article class="feature animate-this">
	{#if order}
		<span class="feature-count">{order}</span>
	{/if}
	<div class="feature-content">
		{#if title}
			<h3>{title}</h3>
		{/if}
		{#if content}
			<p>{content}</p>
		{/if}

		<slot name="title" />
		<slot name="content" />
		<slot />
	</div>
</article>
