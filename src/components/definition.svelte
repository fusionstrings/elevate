<style>

:global(dt) {
	margin: 0;
	color: var(--text-color-dt);
}

dd {
	margin: 0 0 0 2rem;
}
/**
 * line definition style
 */
.lining dt,
.lining dd {
	display: inline;
	margin: 0;
}

.lining dt + dt:before,
.lining dd + dt:before {
	content: "\A";
	white-space: pre;
}

.lining dd + dd:before {
	content: ", ";
}

.lining dd + dd:before {
	content: ", ";
}

.lining dd:before {
	content: ": ";
	margin-left: -0.2em;
}

/**
 * dictionary definition style
 */
.dictionary-style dt {
	display: inline;
	counter-reset: definitions;
}

.dictionary-style dt + dt:before {
	content: ", ";
	margin-left: -0.2em;
}

.dictionary-style dd {
	display: block;
	counter-increment: definitions;
}

.dictionary-style dd:before {
	content: counter(definitions, decimal) ". ";
}


</style>