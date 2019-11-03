<script>
	export let lining = false;
	export let dictionary = false;
</script>

<style>
	:global(dt) {
		margin: 0;
		color: var(--text-color-dt);
	}

	:global(dd) {
		margin: 0 0 0 2rem;
	}
	/**
 * line definition style
 */
	:global(.lining dt, .lining dd) {
		display: inline;
		margin: 0;
	}

	:global(.lining dt + dt:before, .lining dd + dt:before) {
		content: '\A';
		white-space: pre;
	}

	:global(.lining dd + dd:before) {
		content: ', ';
	}

	:global(.lining dd + dd:before) {
		content: ', ';
	}

	:global(.lining dd:before) {
		content: ': ';
		margin-left: -0.2em;
	}

	/**
 * dictionary definition style
 */
	:global(.dictionary dt) {
		display: inline;
		counter-reset: definitions;
	}

	:global(.dictionary dt + dt:before) {
		content: ', ';
		margin-left: -0.2em;
	}

	:global(.dictionary dd) {
		display: block;
		counter-increment: definitions;
	}

	:global(.dictionary dd:before) {
		content: counter(definitions, decimal) '. ';
	}
</style>

<dl class:lining class:dictionary>
	<slot />
</dl>
