<script>
	import Logo from '../components/logo.svelte';
	import Nav from '../components/nav.svelte';
	import NavExtra from '../components/nav-extra.svelte';
	import Header from '../components/header.svelte';

	let navList = [
		{ href: '#intro', title: 'Home', label: 'Home' },
		{ href: '#features', title: 'Features', label: 'Features' },
		{ href: '#infos', title: 'Product Info', label: 'Product Info' },
		{ href: '#stats', title: 'Stats', label: 'Stats' },
		{ href: '#pricing', title: 'Pricing', label: 'Pricing' },
		{ href: '#testimonials', title: 'Testimonials', label: 'Testimonials' },
		{ href: '#download', title: 'Download', label: 'Download' },
		{ href: '#subscribe', title: 'Newsletter', label: 'Newsletter' }
	];
	export let segment;
</script>

<Header>
	<Logo  href=".">Elevate</Logo>
	<Nav {segment} {navList}>
		<NavExtra />
	</Nav>
</Header>

<main>
	<slot />
</main>
