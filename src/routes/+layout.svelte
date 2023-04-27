<script>
  import '../assets/css/global.css';
  import Footer from '../lib/Footer.svelte';

  import Navigation from '../lib/Navigation.svelte';
  import PageLoader from '../lib/PageLoader.svelte';
</script>

<PageLoader />
<div class="app">
  <Navigation />

  <slot />
  <Footer />
</div>

<style>
</style>
