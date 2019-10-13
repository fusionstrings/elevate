<style>
	/* ===================================================================
 * 09. header styles - (_layout.scss)
 *
 * ------------------------------------------------------------------- */
	header {
		width: 100%;
		height: 72px;
		position: fixed;
		left: 0;
		top: 0;
		z-index: 700;
		background: transparent;
	}
	/* ------------------------------------------------------------------- 
 * responsive:
 * header section 
 * ------------------------------------------------------------------- */
	@media only screen and (max-width: 768px) {
		:global(header .logo) {
			top: 33px;
		}
	}
</style>

<header class="main-header">
	<slot name="logo" />
	<slot name="nav" />
	<slot />
</header>
