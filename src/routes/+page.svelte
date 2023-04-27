<script>
  import { onMount } from 'svelte';
  import { smoothScroll } from '../hooks/lenis/smoothScroll';
  /* component */
  import Hero from '../lib/Hero.svelte';
  import Animation from '../lib/Animation.svelte';
  import Tech from '../lib/Tech.svelte';
  import Showcase from '../lib/Showcase.svelte';

  onMount(() => {
    smoothScroll();
  });
</script>

<Hero />
<Showcase />
<Animation />

<Tech />

<style></style>
