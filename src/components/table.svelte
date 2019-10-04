<script>
	export let responsive;
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

	:global(th:first-child, td:first-child) {
		padding-left: 0;
	}

	:global(th:last-child, td:last-child) {
		padding-right: 0;
	}

	:global(.table-responsive) {
		overflow-x: auto;
		-webkit-overflow-scrolling: touch;
	}
</style>

<table class:responsive />
