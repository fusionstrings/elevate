<script>
	export let responsive = true;
	export let compact = false;
	export let width = '100%';
</script>

<style>
	/* ------------------------------------------------------------------- 
 * tables - (_document-setup.scss)    
 * ------------------------------------------------------------------- */
	:global(table) {
		border-width: 0;
		width: 100%;
		max-width: 100%;
		font-family: var(--font-family-table);
	}

	:global(th, td) {
		padding: 1.5rem 3rem;
		text-align: left;
		border-bottom: 1px solid var(--border-color-table);
	}

	:global(th) {
		color: black;
		font-weight: var(--font-weight-black);
	}

	:global(td) {
		line-height: 1.5;
	}

	:global(th:first-child, td:first-child, .compact table th:first-child, .compact table td:first-child) {
		padding-left: 0;
	}

	:global(th:last-child, td:last-child, .compact table th:last-child, .compact table td:last-child) {
		padding-right: 0;
	}

	:global(.responsive) {
		overflow-x: auto;
		-webkit-overflow-scrolling: touch;
	}
	.compact{
		overflow: hidden;
		overflow-y: auto;
		font-size: 1.2rem;
	}
	:global(.compact table th){
		padding: 0.5rem;
	}
	:global(.compact table td){
		line-height: 0.2;
		padding: 1rem 0.5rem;
		border-bottom: 1px solid rgb(232, 232, 232, 0.25);
	}
	:global(td.right){
		text-align: right;
	}
</style>

<div class:responsive class:compact>
	<table width={width}>
		<slot />
	</table>
</div>
