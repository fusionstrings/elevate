<script>
	import Hero from '../components/hero.svelte';
	import Features from '../components/features.svelte';
	import Lead from '../components/lead.svelte';
	import SectionLead from '../components/section-lead.svelte';
	import FeatureBlock from '../components/feature-block.svelte';
	import FeatureList from '../components/feature-list.svelte';

	import Informations from '../components/informations.svelte';
	import Stats from '../components/stats.svelte';
	import Plans from '../components/plans.svelte';
	import Testimonials from '../components/testimonials.svelte';
	import Callback from '../components/callback.svelte';
	import Subscription from '../components/subscription.svelte';
	import Footer from '../components/footer.svelte';
	import ButtonGotoTop from '../components/button-goto-top.svelte';

	function onClick() {
		console.log('event');
	}
</script>

<svelte:head>
	<title>Elevate</title>
</svelte:head>
<Hero
	heading="The perfect template to present your awesome product."
	subheading="Introducing Elevate"
	actions={[{ label: 'Features', href: 'features' }, { label: 'Download', onClick: onClick }]}>

	<img src="images/app-screenshot-big.jpg" alt="" class="animate-intro" />
</Hero>

<Features>
	<SectionLead title="Features You'll Love.">
		<Lead>
			Lorem ipsum Tempor do Excepteur nulla aute deserunt reprehenderit
			aute commodo aliquip laboris velit eu esse exercitation ex fugiat
			pariatur aute consequat. Lorem ipsum Fugiat mollit quis qui. Lorem
			ipsum Duis Excepteur Duis magna fugiat incididunt qui id quis dolor
			nisi irure proident labore ut in incididunt eiusmod est anim.
		</Lead>
	</SectionLead>

	<FeatureList>
		<FeatureBlock order="01.">
			<h3>Fully Resposive</h3>
			<p>
				Sed ut perspiciatis unde omnis iste natus error sit voluptatem
				accusantium doloremque laudantium, totam rem aperiam, eaque ipsa
				quae ab illo inventore veritatis et quasi architecto beatae
				vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia
				voluptas sit aspernatur aut odit aut fugit.
			</p>
		</FeatureBlock>
		<!-- /bgrid -->

		<FeatureBlock order="02." title="Retina Ready">
			<p>
				Sed ut perspiciatis unde omnis iste natus error sit voluptatem
				accusantium doloremque laudantium, totam rem aperiam, eaque ipsa
				quae ab illo inventore veritatis et quasi architecto beatae
				vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia
				voluptas sit aspernatur aut odit aut fugit.
			</p>
		</FeatureBlock>
		<!-- /bgrid -->

		<FeatureBlock order="03." title="Stylish Design">
			<p name="content">
				Sed ut perspiciatis unde omnis iste natus error sit voluptatem
				accusantium doloremque laudantium, totam rem aperiam, eaque ipsa
				quae ab illo inventore veritatis et quasi architecto beatae
				vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia
				voluptas sit aspernatur aut odit aut fugit.
			</p>
		</FeatureBlock>
		<!-- /bgrid -->

		<FeatureBlock
			order="04."
			title="Clean Code"
			content="Sed ut perspiciatis unde omnis iste natus error sit
			voluptatem accusantium doloremque laudantium, totam rem aperiam,
			eaque ipsa quae ab illo inventore veritatis et quasi architecto
			beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia
			voluptas sit aspernatur aut odit aut fugit." />
		<!-- /bgrid -->

		<FeatureBlock order="05.">
			<h3 name="title">Easy To Customize</h3>
			<p name="content">
				Sed ut perspiciatis unde omnis iste natus error sit voluptatem
				accusantium doloremque laudantium, totam rem aperiam, eaque ipsa
				quae ab illo inventore veritatis et quasi architecto beatae
				vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia
				voluptas sit aspernatur aut odit aut fugit.
			</p>
		</FeatureBlock>
		<!-- /bgrid -->

		<FeatureBlock>
			<span class="feature-count">06.</span>
			<h3>Free of Charge</h3>
			<p>
				Sed ut perspiciatis unde omnis iste natus error sit voluptatem
				accusantium doloremque laudantium, totam rem aperiam, eaque ipsa
				quae ab illo inventore veritatis et quasi architecto beatae
				vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia
				voluptas sit aspernatur aut odit aut fugit.
			</p>
		</FeatureBlock>
		<!-- /bgrid -->
	</FeatureList>
</Features>

<Informations />

<Stats />

<Plans />

<Testimonials />

<Callback />

<Subscription />
<Footer />
<ButtonGotoTop />
