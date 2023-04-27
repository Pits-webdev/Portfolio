<script>
  import { animate, timeline } from 'motion';
  import { onMount } from 'svelte';

  $: count = 0;
  let loaderDuration = 4;

  onMount(() => {
    animate(
      (progress) => {
        count = progress.toFixed(1) * 100;
      },
      {
        duration: 2.5,
      },
      { easing: 'ease-in' }
    );

    const sequence = [
      ['.loader_head', { y: '-100%' }, { duration: 0.5 }],
      ['.loader_bottom', { y: '100%' }, { duration: 0.5 }],
      ['.loader', { display: 'none' }, { duration: 0 }],
      ['.app', { display: 'block' }],
    ];

    timeline(sequence, { delay: 2 }, { ease: 'ease-in-out' });
  });
</script>

<div class="loader">
  <div class="loader_head">
    <div class="loader_progress_bar" style="width: {count}%" />
    <div class="container">
      <h1 class="hl">peter web<br />developer</h1>

      <h2>didital<br />creater</h2>
    </div>
  </div>
  <div class="loader_bottom">
    <div class="container">
      <p class="counter">{count}</p>
    </div>
  </div>
</div>

<style>
  .loader {
    width: 100%;
    height: 100vh;
    position: absolute;
    left: 0;
    top: 0;
    overflow: hidden;
    background-color: var(--black);
    z-index: 9999;
  }

  .loader_head {
    position: relative;
    width: 100%;
    height: 10rem;
    border-bottom: 4px solid var(--white);
    background-color: var(--black);
  }

  .loader_progress_bar {
    position: absolute;
    width: 20%;
    height: 100%;
    background-color: var(--primary);
    transition: all 0.2s;
  }

  .loader_head .container {
    width: 100%;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    z-index: 2;
    color: var(--primary);
    padding: 0 2rem;
  }

  .container h1,
  h2 {
    mix-blend-mode: difference;
    z-index: 3;
    font-family: 'Syncopate';
    font-size: 2rem;
  }

  .loader_bottom {
    position: relative;
    width: 100%;
    height: calc(100% - 10rem);
  }

  .loader_bottom .container {
    position: relative;
    width: 100%;
    height: 100%;
  }

  .loader_bottom .counter {
    width: 55rem;
    height: 30rem;
    font-size: 12rem;
    position: absolute;
    bottom: 0;
    right: 0;
    display: grid;
    place-items: center;
    color: var(--primary);
    font-weight: 900;
    font-family: 'Syncopate';
    font-weight: 700;
  }
</style>
