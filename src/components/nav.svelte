<script>
	let toggle = false;
	export let navList = [];
	export let segment;
	function onToggle() {
		toggle = !toggle;
	}
</script>

<style>
	/* ------------------------------------------------------------------- 
 * menu toggle - (_layout.css) 
 * ------------------------------------------------------------------- */
	.menu-toggle {
		width: 42px;
		height: 42px;
		display: block;
		outline: 0;
		background: #111111;
		margin-right: 20px;
		transition: transform 0.4s ease-in-out;
		transform: translateZ(0);
		-webkit-transform: translateZ(0);
		backface-visibility: hidden;
		-webkit-backface-visibility: hidden;
	}

	.menu-toggle span {
		display: block;
		background-color: #ffffff;
		width: 24px;
		height: 3px;
		margin-top: -1.5px;
		position: absolute;
		right: 9px;
		top: 50%;
		bottom: auto;
		left: auto;
		font: 0/0 a;
		text-shadow: none;
		color: transparent;
		transition: background 0.2s ease-in-out;
	}

	.menu-toggle span::before,
	.menu-toggle span::after {
		content: '';
		width: 100%;
		height: 100%;
		background-color: inherit;
		position: absolute;
		left: 0;
		transition: all 0.2s ease-in-out;
	}

	.menu-toggle span::before {
		top: -8px;
	}

	.menu-toggle span::after {
		bottom: -8px;
	}

	/* menu is open */
	.menu-toggle-open {
		transform: translateX(-240px);
	}

	/* is clicked */
	.menu-clicked span {
		background-color: rgba(255, 255, 255, 0);
	}

	.menu-clicked span::before,
	.menu-clicked span::after {
		background-color: white;
	}

	.menu-clicked span::before {
		top: 0;
		transform: rotate(45deg);
	}

	.menu-clicked span::after {
		bottom: 0;
		transform: rotate(-45deg);
	}

	/* ------------------------------------------------------------------- 
 * off-canvas menu - (_layout.scss) 
 * ------------------------------------------------------------------- */

	nav {
		background: #111111;
		color: rgba(255, 255, 255, 0.25);
		font-size: 1.5rem;
		line-height: 1.6;
		padding: 3.6rem 3rem;
		height: 100%;
		width: 240px;
		position: fixed;
		right: 0;
		top: 0;
		visibility: hidden;
		z-index: 800;
		overflow-y: auto;
		-webkit-transform: translateZ(0);
		-webkit-transform: translateX(100%);
		-ms-transform: translateX(100%);
		transform: translateX(100%);
		-moz-transition: all 0.4s ease-in-out;
		-o-transition: all 0.4s ease-in-out;
		-webkit-transition: all 0.4s ease-in-out;
		-ms-transition: all 0.4s ease-in-out;
		transition: all 0.4s ease-in-out;
	}

	nav a,
	nav a:visited {
		color: rgba(255, 255, 255, 0.5);
	}

	nav a:hover,
	nav a:focus,
	nav a:active {
		color: white;
	}

	:global(nav.menu-open h3) {
		color: white;
		font-weight: var(--font-weight-bold);
		font-size: 1.6rem;
		line-height: 1.5;
		margin-bottom: 1.5rem;
	}

	.nav-list {
		margin: 1.8rem 0 1.5rem 0;
		padding: 0 0 1.5rem 0;
		list-style: none;
		line-height: 3.6rem;
	}

	.nav-list li {
		padding-left: 0;
	}

	.nav-list li a {
		color: rgba(255, 255, 255, 0.25);
	}

	.nav-list li a:hover,
	.nav-list li a:focus {
		color: white;
	}
	/* menu is open */
	.menu-open {
		-webkit-transform: translateX(0);
		-ms-transform: translateX(0);
		transform: translateX(0);
		visibility: visible;
		-webkit-overflow-scrolling: touch;
	}
</style>

{#if navList.length > 0}
	<span
		class={toggle ? 'menu-toggle menu-toggle-open menu-clicked' : 'menu-toggle'}
		on:click={onToggle}>
		<span>Menu</span>
	</span>

	{#if toggle}
		<nav class="menu-open">

			<h3>Navigation</h3>

			<ul class="nav-list">
				{#each navList as { href, label, title, activePath, rel }}
					<li>
						<a {href} {title} {rel} class:selected='{segment === href}'>{label}</a>
					</li>
				{/each}
			</ul>
			<slot />
		</nav>
	{/if}
{/if}
