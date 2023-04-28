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

            <span class="icon">
              <img src="images/eye_yellow.svg" alt="eye" />
              <img src="images/eye_black.svg" alt="eye" />
            </span>
          </HeroCard>
        </div>

        <div class="card">
          <HeroCard />
        </div>

        <div class="card bg">
          <HeroCard>
            <h3>Web development</h3>
            <p>New tech for maximal performence</p>

            <span class="icon">
              <img
                class="sm"
                src="images/performence_yellow.svg"
                alt="performence"
              />
              <img
                class="sm"
                src="images/performence_black.svg"
                alt="performence"
              />
            </span>
          </HeroCard>
        </div>

        <div class="card">
          <HeroCard />
        </div>

        <div class="card bg">
          <HeroCard>
            <h3>All in one</h3>
            <p>Let's bring it together</p>

            <span class="icon">
              <img src="images/amor_yellow.svg" alt="amor" />
              <img src="images/amor_black.svg" alt="amor" /></span
            >
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
    display: flex;
    align-items: flex-end;
    bottom: 2rem;
    width: 4rem;
    height: 4rem;
  }

  .card .icon img {
    position: absolute;
    width: 100%;
  }
  .card .icon .sm {
    width: 70%;
  }

  .card.bg {
    background-color: var(--primary);
  }

  /* hover effext */
  .card.bg:hover {
    color: var(--primary);
    background-color: var(--black);
  }
  .card.bg:hover .icon img:last-child {
    opacity: 0;
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
