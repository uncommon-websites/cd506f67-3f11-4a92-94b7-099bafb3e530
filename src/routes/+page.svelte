<script>
  import Header from '$lib/components/Header.svelte';
  import Hero from '$lib/components/Hero.svelte';
  import Logos from '$lib/components/Logos.svelte';
  import ValueProp from '$lib/components/ValueProp.svelte';
  import Products from '$lib/components/Products.svelte';
  import Features from '$lib/components/Features.svelte';
  import Testimonial from '$lib/components/Testimonial.svelte';
  import Footer from '$lib/components/Footer.svelte';
</script>

<svelte:head>
  <title>Select - Premium Banking Without the Friction</title>
  <meta name="description" content="Select delivers premium banking services through stablecoin infrastructure, eliminating traditional banking friction and fees. Global banking access for high-net-worth individuals and businesses." />
  <meta property="og:title" content="Select - Premium Banking Without the Friction" />
  <meta property="og:description" content="Premium banking built on stablecoin infrastructure. No hidden fees, no delays, no geographic limitations." />
  <meta property="og:type" content="website" />
  <meta name="twitter:card" content="summary_large_image" />
  <meta name="twitter:title" content="Select - Premium Banking Without the Friction" />
  <meta name="twitter:description" content="Premium banking built on stablecoin infrastructure. No hidden fees, no delays, no geographic limitations." />
</svelte:head>

<Header />

<main class="bg-white overflow-hidden">
  <Hero />
  <Logos />
  <ValueProp />
  <Products />
  <Features />
  <Testimonial />
</main>

<Footer />

