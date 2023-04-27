<script>
  import HeroCard from './HeroCard.svelte';
</script>

<header>
  <div class="hero_template container_xl">
    <div class="hero_block">
      <div class="headline">
        <h1>
          Development <br />
          <span class="col_span"
            ><svg
              xmlns="http://www.w3.org/2000/svg"
              xml:space="preserve"
              width="90.266"
              height="42.828"
              viewBox="0 0 23.883 11.332"
              ><g transform="translate(-125.783 -102.213)"
                ><path
                  d="M126.325 107.851s6.228-4.054 9.811-4.918a6.17 6.17 0 0 1 2.794-.032c3.587.83 9.778 4.95 9.778 4.95s-5.759 4.075-9.146 4.924a8.042 8.042 0 0 1-3.792 0c-3.477-.847-9.445-4.924-9.445-4.924z"
                  style="fill:none;stroke:#000;stroke-width:1.0843;stroke-dasharray:none"
                /><ellipse
                  cx="137.558"
                  cy="107.786"
                  rx="4.504"
                  ry="4.87"
                  style="fill:none;stroke:#000;stroke-width:1.3979;stroke-dasharray:none"
                /><ellipse
                  cx="137.558"
                  cy="107.837"
                  rx="2.242"
                  ry="2.337"
                  style="fill:#000;stroke:none;stroke-width:1.61998;stroke-dasharray:none"
                /></g
              ></svg
            > of the
          </span>
          <br />

          future
        </h1>
      </div>

      <div class="content">
        <span class="img">
          <img src="images/peter.png" alt="portfolio" />
        </span>
        <p>
          I'm Peter, I help clients to achieve greater visibility,I'm Peter, I
          help clients to achieve greater visibility help clients to achieve
          greater visibility
        </p>
      </div>
    </div>

    <div class="hero_block">
      <div class="cards">
        <div class="card bg">
          <HeroCard>
            <h3>Web design</h3>
            <p>Modern design, tailored to your brand</p>

            <span class="icon"
              ><svg
                xmlns="http://www.w3.org/2000/svg"
                xml:space="preserve"
                width="90.266"
                height="42.828"
                viewBox="0 0 23.883 11.332"
                ><g transform="translate(-125.783 -102.213)"
                  ><path
                    class="eye_stroke"
                    d="M126.325 107.851s6.228-4.054 9.811-4.918a6.17 6.17 0 0 1 2.794-.032c3.587.83 9.778 4.95 9.778 4.95s-5.759 4.075-9.146 4.924a8.042 8.042 0 0 1-3.792 0c-3.477-.847-9.445-4.924-9.445-4.924z"
                  /><ellipse
                    cx="137.558"
                    cy="107.786"
                    rx="4.504"
                    ry="4.87"
                    style="fill:none;stroke:#000;stroke-width:1.3979;stroke-dasharray:none"
                  /><ellipse
                    class="eye_stroke"
                    cx="137.558"
                    cy="107.837"
                    rx="2.242"
                    ry="2.337"
                  /></g
                ></svg
              ></span
            >
          </HeroCard>
        </div>

        <div class="card">
          <HeroCard />
        </div>

        <div class="card bg">
          <HeroCard>
            <h3>Web development</h3>
            <p>New tech for maximal performence</p>

            <span class="icon"
              ><svg
                xmlns="http://www.w3.org/2000/svg"
                xml:space="preserve"
                width="48.985"
                height="48.965"
                viewBox="0 0 12.961 12.955"
                ><path
                  class="one"
                  d="M123.975 101.421h.289v1.325h-.289z"
                  style="fill:#000;stroke:#000;stroke-width:.749658"
                  transform="translate(-122.778 -90.288)"
                /><path
                  class="two"
                  d="M126.744 100.482h.229v2.208h-.229z"
                  style="fill:#000;stroke:#000;stroke-width:.861432"
                  transform="translate(-122.778 -90.288)"
                /><path
                  class="three"
                  d="M129.519 98.477h.144v4.239h-.144z"
                  style="fill:#000;stroke:#000;stroke-width:.946492"
                  transform="translate(-122.778 -90.288)"
                /><path
                  class="four"
                  d="M132.311 97.36h.127v5.383h-.127z"
                  style="fill:#000;stroke:#000;stroke-width:1.00012"
                  transform="translate(-122.778 -90.288)"
                /><path
                  class="five"
                  d="M135.127 95.204h.096v7.524h-.096z"
                  style="fill:#000;stroke:#000;stroke-width:1.03056"
                  transform="translate(-122.778 -90.288)"
                /><path
                  class="six"
                  d="m122.778 98.812 3.296-4.002 1.148 1.005 2.835-3.104 1.174 1.61 2.22-2.727-.903-1.043 2.766-.263-.561 2.795-.748-.815-2.8 3.256-1.148-1.51-2.91 3.135-.883-.846-2.74 3.143z"
                  style="fill:#000;stroke:none;stroke-width:.925658"
                  transform="translate(-122.778 -90.288)"
                /></svg
              ></span
            >
          </HeroCard>
        </div>

        <div class="card">
          <HeroCard />
        </div>

        <div class="card bg">
          <HeroCard>
            <h3>All in one</h3>
            <p>Let's bring it together</p>

            <span class="icon"><img src="images/amor.svg" alt="" /></span>
          </HeroCard>
        </div>

        <div class="card">
          <HeroCard />
        </div>
      </div>
    </div>
  </div>

  <div class="marquee">
    <div class="marquee_content">
      <span class="marquee_inner">make your brand bigger</span>
      <span class="marquee_inner">make your brand bigger</span>
      <span class="marquee_inner">make your brand bigger</span>
    </div>

    <div class="marquee_content">
      <span class="marquee_inner">make your brand bigger</span>
      <span class="marquee_inner">make your brand bigger</span>
      <span class="marquee_inner">make your brand bigger</span>
    </div>
  </div>
</header>

<style>
  header {
    width: 100%;
    height: 91vh;
    padding: calc(91vh - 78vh) 0;
  }

  .hero_template {
    height: max-content;
    display: flex;
    justify-content: space-between;
    gap: 2rem;
  }

  /* left */
  .hero_block {
    width: 100%;
    height: max-content;
    flex: 1;
  }

  .hero_block h1 {
    font-size: 6rem;
    line-height: 1.8;
  }

  .headline {
    width: 100%;
    height: max-content;
  }

  .content {
    height: max-content;
    max-width: 60rem;
    display: flex;
    gap: 2rem;
  }

  .content .img {
    display: inline-block;
    width: 3rem;
    height: 3rem;
    border: 1px solid var(--black);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .content .img img {
    width: 3rem;
    height: 3rem;
    padding: 0.5rem;
  }
  .content p {
    line-height: 1.6;
  }

  .hero_block h1 .col_span {
    border: 1px solid var(--black);
    border-radius: 3rem;
    padding: 0 2rem;
    background-color: var(--primary);
  }

  span {
    display: inline-block;
  }

  /* right */
  .cards {
    width: 100%;
    height: max-content;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
  }

  .card {
    position: relative;
    width: 100%;
    height: 200px;
    border: 1px solid var(--black);
    border-radius: 2rem;
    padding: 2rem;
    transition: all 0.1s ease;
  }

  .card .icon {
    position: absolute;
    bottom: 2rem;
  }

  .card .icon svg {
    width: 50%;
    height: 50%;
  }

  .card.bg {
    background-color: var(--primary);
  }
  .card.bg:hover {
    color: var(--primary);
    background-color: var(--black);
  }

  /* hover effext */

  .card.bg:hover svg path {
    fill: var(--black);
    stroke: var(--black);
  }

  .card.bg .eye_stroke {
    fill: none;
    stroke: var(--black);
    stroke-width: 1.0843;
    stroke-dasharray: none;
  }

  .card.bg:hover .eye_stroke {
    fill: var(--primary);
    stroke: var(--primary);
  }

  .card h3 {
    font-size: 2rem;
    font-weight: 700;
    margin-bottom: 1rem;
  }

  /* marquee */
  .marquee {
    --gap: 20rem;
    display: flex;
    overflow: hidden;
    user-select: none;
    gap: var(--gap);
    margin-top: calc(91vh - 74vh);
  }

  .marquee_content {
    flex-shrink: 0;
    display: flex;
    justify-content: space-around;
    min-width: 100%;
    gap: var(--gap);
    animation: scroll 22s linear infinite;
  }

  .marquee_inner {
    font-size: 4rem;
    font-family: 'Syncopate';
    font-weight: 700;
    background-color: var(--black);
    color: var(--primary);
    border-radius: 1rem;
    padding: 1rem 2rem;
  }
  @keyframes scroll {
    from {
      transform: translateX(0);
    }
    to {
      transform: translateX(calc(-100% - var(--gap)));
    }
  }
</style>
