<style>
	/* ===================================================================
 * 09. header styles - (_layout.scss)
 *
 * ------------------------------------------------------------------- */
	:global(body){
		--header-height: 72px;
	}
	header {
		height: var(--header-height);
		z-index: 700;
		position: sticky;
		top: 0px;
		background: transparent;
		display: flex;
		justify-content: space-between;
		align-items: center;
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
	<slot />
	<slot name="nav" />
</header>
