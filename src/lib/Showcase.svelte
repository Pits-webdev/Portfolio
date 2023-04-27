<script>
  import { scroll, animate, ScrollOffset } from 'motion';
  import { onMount } from 'svelte';

  onMount(() => {
    const sectionPin = document.querySelector('.showcase');

    scroll(
      animate('.scroll', {
        transform: ['translateX(0)', `translateX(calc(-100% + 100vw))`],
      }),
      {
        target: sectionPin,
        offset: ScrollOffset.enter,
      }
    );
  });
</script>

<section>
  <div class="showcase container_xl">
    <div class="showcase_template">
      <h2>Showcase</h2>
      <div class="scroll">
        <div class="case">
          <video src="videos/car.mp4" muted playsinline controls id="car">
            <track kind="captions" />
          </video>
        </div>
        <div class="case">
          <img src="images/socialProject.png" alt="webside" />
        </div>
        <div class="case">
          <img src="images/Gym.png" alt="webside" />
        </div>
      </div>
    </div>
  </div>
</section>

<style>
  .showcase {
    width: 100%;
    height: calc(100vh * 3);
    overflow-x: clip;
  }

  .showcase_template {
    position: sticky;
    top: 0;
    height: 100vh;
  }

  h2 {
    padding-top: 10rem;
    margin-left: 2.5vw;
  }

  .scroll {
    margin-top: 5rem;
    width: 300vw;
    display: flex;
    height: 600px;
  }

  .case {
    display: grid;
    place-content: center;
    width: 100%;
    height: 100%;
    position: sticky;
    top: 0;
    padding: 10rem 0;
  }

  .case img,
  .case video {
    width: 100%;
    height: 600px;
    border-radius: 2rem;
  }
</style>
