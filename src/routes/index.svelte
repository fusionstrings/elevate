<script>
  import Hero from "../components/hero.svelte";
  import Features from "../components/features.svelte";
  import Informations from "../components/informations.svelte";
  import Stats from "../components/stats.svelte";
  import Plans from "../components/plans.svelte";
  import Testimonials from "../components/testimonials.svelte";
  import Callback from "../components/callback.svelte";
  import Subscription from "../components/subscription.svelte";
  import Footer from "../components/footer.svelte";
  import ButtonGotoTop from "../components/button-goto-top.svelte";

  function onClick() {
    console.log("event");
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

<Features />

<Informations />

<Stats />

<Plans />

<Testimonials />

<Callback />

<Subscription />
<Footer />
<ButtonGotoTop />
