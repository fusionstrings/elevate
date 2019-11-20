<script>
	export let href;
</script>

<style>
	/* ------------------------------------------------------------------- 
 * header logo - (_layout.css) 
 * ------------------------------------------------------------------- */
	.logo {
		margin-left: 26px;
		margin-top: 30px;
	}

	.logo a {
		display: block;
		margin: 0;
		padding: 0;
		outline: 0;
		border: none;
		width: 96px;
		height: 20px;
		background: url('../images/logo.png') no-repeat center;
		background-size: 96px 20px;
		font: 0/0 a;
		text-shadow: none;
		color: transparent;
		-moz-transition: all 0.5s ease-in-out;
		-o-transition: all 0.5s ease-in-out;
		-webkit-transition: all 0.5s ease-in-out;
		-ms-transition: all 0.5s ease-in-out;
		transition: all 0.5s ease-in-out;
	}
</style>

<div class="logo">
	<a {href}>
		<slot />
	</a>
</div>
