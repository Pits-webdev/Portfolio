<script>
  import Accordion from './Accordion.svelte';
</script>

<section>
  <div class="tech container_xl">
    <h2>What tech i work with</h2>

    <div class="tech_template">
      <div class="tech_block">
        <div class="cards">
          <span class="tech_card card_light">HTML 65%</span>
          <span class="tech_card card_dark">CSS 90%</span>
          <span class="tech_card card_light">Javascript 80%</span>

          <h4>Framework</h4>
          <span class="tech_card card_dark">React & Next.js 60%</span>
          <span class="tech_card card_light">Svelte & Sveltekit 75%</span>

          <h4>Libary</h4>
          <span class="tech_card card_dark">Three.js 15%</span>
        </div>
      </div>

      <!-- Accordion -->
      <div class="tech_block">
        <Accordion>
          <strong slot="tech">HTML</strong>
          <p slot="desc">app Sceleton</p>
        </Accordion>

        <Accordion>
          <strong slot="tech">CSS</strong>
          <p slot="desc">style your app</p>
        </Accordion>

        <Accordion>
          <strong slot="tech">Javascript</strong>
          <p slot="desc">dynamic for your app</p>
        </Accordion>

        <Accordion>
          <strong slot="tech">Framework</strong>
          <p slot="desc">Framework for your app</p>
        </Accordion>

        <Accordion>
          <strong slot="tech">Libary</strong>
          <p slot="desc">Libary Three.js for your app</p>
        </Accordion>
      </div>
    </div>
  </div>
</section>

<style>
  .tech {
    margin-top: 12rem;
  }

  .tech_template {
    width: 100%;
    display: flex;
    gap: 2rem;
    margin-top: 5rem;
  }

  .tech_block {
    flex: 1;
  }

  .cards {
    width: 100%;
  }

  .cards h4 {
    margin: 3rem 0 1rem;
  }

  .tech_card {
    display: block;
    width: max-content;
    border: 1px solid var(--black);
    padding: 1rem 2rem;
    margin-bottom: 1rem;
    border-radius: 1rem;
    font-size: 2rem;
  }

  .tech_card:last-child {
    margin-bottom: 0;
  }
  .card_light {
    background-color: var(--primary);
    color: var(--black);
  }

  .card_dark {
    background-color: var(--black);
    color: var(--primary);
  }
</style>
