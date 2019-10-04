<script>
	export let disc;
	export let list = [];
	export let type = 'ul';
</script>

<style>
	/* ------------------------------------------------------------------- 
 * Lists - (_document-setup.scss)  
 * ------------------------------------------------------------------- */
	:global(ol) {
		list-style: decimal;
	}

	:global(ul) {
		list-style: disc;
	}

	:global(li) {
		display: list-item;
	}

	:global(ol, ul) {
		margin-left: 1.7rem;
	}

	:global(ul li) {
		padding-left: 0.4rem;
	}

	:global(ul ul, ul ol, ol ol, ol ul) {
		margin: 0.6rem 0 0.6rem 1.7rem;
	}

	:global(ul.disc li) {
		display: list-item;
		list-style: none;
		padding: 0 0 0 0.8rem;
		position: relative;
	}

	:global(ul.disc li::before) {
		content: '';
		display: inline-block;
		width: 8px;
		height: 8px;
		border-radius: 50%;
		background: var(--list-bullet-color);
		position: absolute;
		left: -17px;
		top: 11px;
		vertical-align: middle;
	}
</style>

{#if type === 'ol'}
	<ol class:disc>
		{#if list.length > 0}
			{#each list as li}
				<li>{li}</li>
			{/each}
		{/if}
		<slot />
	</ol>
{:else}
	<ul class:disc>
		{#if list.length > 0}
			{#each list as li}
				<li>{li}</li>
			{/each}
		{/if}
		<slot />
	</ul>
{/if}
