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
  <title>Select - Operate Globally with Stablecoin Infrastructure</title>
  <meta name="description" content="Select allows businesses and individuals to operate globally with ease through stablecoin infrastructure. Receive fiat payments, convert to stablecoins, and pay suppliers worldwide." />
  <meta property="og:title" content="Select - Operate Globally with Stablecoin Infrastructure" />
  <meta property="og:description" content="Receive fiat payments, convert to stablecoins at institutional rates, and pay suppliers worldwide using local rails. Powered by MoonPay." />
  <meta property="og:type" content="website" />
  <meta name="twitter:card" content="summary_large_image" />
  <meta name="twitter:title" content="Select - Operate Globally with Stablecoin Infrastructure" />
  <meta name="twitter:description" content="Receive fiat payments, convert to stablecoins at institutional rates, and pay suppliers worldwide using local rails. Powered by MoonPay." />
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

