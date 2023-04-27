<script></script>

<section>
  <div class="animation container_xl">
    <h2>Web animations</h2>

    <p>Maximum performance</p>

    <div class="animation_template">
      <!-- square -->
      <div class="animation_block">
        <div class="square">
          <span />
          <span />
          <span />
          <span />
          <span />
          <span />
          <span />
          <span />
          <span />
          <span />
          <span />
          <span />
          <span />
          <span />
          <span />
          <span />
          <span />
          <span />
        </div>
      </div>
      <!-- circle -->
      <div class="animation_block">
        <div class="circle eye">
          <h1 style="color: var(--primary)">eye</h1>
        </div>
      </div>
      <div class="animation_block">
        <div class="circle">
          <span />
          <span />
          <span />
          <span />
          <span />
          <span />
          <span />
          <span />
          <span />
          <span />
        </div>
      </div>
    </div>
  </div>
</section>

<style>
  .animation {
    margin-top: 12rem;
  }

  .animation h2 {
    margin-bottom: 1rem;
  }

  .animation_template {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 4rem;
    margin-top: 5rem;
  }
  .animation_block {
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: var(--primary);
    border: 1px solid var(--black);
    border-radius: 2rem;
    width: 100%;
    height: 40rem;
    padding: 5rem;
  }

  .animation_block:nth-child(2) {
    background-color: var(--black);
  }

  /* square */

  .square {
    width: 100%;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .square span {
    position: absolute;
    display: block;
    width: 25rem;
    height: 25rem;
    border: 2px solid var(--black);
    animation: square 3s ease-in-out infinite alternate;
  }

  .square span:nth-child(1) {
    animation-name: rotate-1;
  }
  .square span:nth-child(2) {
    animation-name: rotate-2;
  }
  .square span:nth-child(3) {
    animation-name: rotate-3;
  }
  .square span:nth-child(4) {
    animation-name: rotate-4;
  }
  .square span:nth-child(5) {
    animation-name: rotate-5;
  }
  .square span:nth-child(6) {
    animation-name: rotate-6;
  }
  .square span:nth-child(7) {
    animation-name: rotate-7;
  }
  .square span:nth-child(8) {
    animation-name: rotate-8;
  }
  .square span:nth-child(9) {
    animation-name: rotate-9;
  }
  .square span:nth-child(10) {
    animation-name: rotate-10;
  }
  .square span:nth-child(11) {
    animation-name: rotate-11;
  }
  .square span:nth-child(12) {
    animation-name: rotate-12;
  }
  .square span:nth-child(13) {
    animation-name: rotate-13;
  }
  .square span:nth-child(14) {
    animation-name: rotate-14;
  }
  .square span:nth-child(15) {
    animation-name: rotate-15;
  }
  .square span:nth-child(16) {
    animation-name: rotate-16;
  }
  .square span:nth-child(17) {
    animation-name: rotate-17;
  }
  .square span:nth-child(18) {
    animation-name: rotate-18;
  }

  @keyframes rotate-1 {
    100% {
      width: 10rem;
      border-radius: 50%;
      transform: rotate(360deg);
    }
  }

  @keyframes rotate-2 {
    100% {
      width: 10rem;
      border-radius: 50%;
      transform: rotate(350deg);
    }
  }
  @keyframes rotate-3 {
    100% {
      width: 10rem;
      border-radius: 50%;
      transform: rotate(340deg);
    }
  }
  @keyframes rotate-4 {
    100% {
      width: 10rem;
      border-radius: 50%;
      transform: rotate(330deg);
    }
  }
  @keyframes rotate-5 {
    100% {
      width: 10rem;
      border-radius: 50%;
      transform: rotate(320deg);
    }
  }
  @keyframes rotate-6 {
    100% {
      width: 10rem;
      border-radius: 50%;
      transform: rotate(310deg);
    }
  }
  @keyframes rotate-7 {
    100% {
      width: 10rem;
      border-radius: 50%;
      transform: rotate(300deg);
    }
  }
  @keyframes rotate-8 {
    100% {
      width: 10rem;
      border-radius: 50%;
      transform: rotate(290deg);
    }
  }
  @keyframes rotate-9 {
    100% {
      width: 10rem;
      border-radius: 50%;
      transform: rotate(280deg);
    }
  }
  @keyframes rotate-10 {
    100% {
      width: 10rem;
      border-radius: 50%;
      transform: rotate(270deg);
    }
  }
  @keyframes rotate-11 {
    100% {
      width: 10rem;
      border-radius: 50%;
      transform: rotate(260deg);
    }
  }
  @keyframes rotate-12 {
    100% {
      width: 10rem;
      border-radius: 50%;
      transform: rotate(250deg);
    }
  }
  @keyframes rotate-13 {
    100% {
      width: 10rem;
      border-radius: 50%;
      transform: rotate(240deg);
    }
  }
  @keyframes rotate-14 {
    100% {
      width: 10rem;
      border-radius: 50%;
      transform: rotate(230deg);
    }
  }
  @keyframes rotate-15 {
    100% {
      width: 10rem;
      border-radius: 50%;
      transform: rotate(220deg);
    }
  }
  @keyframes rotate-16 {
    100% {
      width: 10rem;
      border-radius: 50%;
      transform: rotate(210deg);
    }
  }
  @keyframes rotate-17 {
    100% {
      width: 10rem;
      border-radius: 50%;
      transform: rotate(200deg);
    }
  }
  @keyframes rotate-18 {
    100% {
      width: 10rem;
      border-radius: 50%;
      transform: rotate(190deg);
    }
  }

  /* circle */
  .circle {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 30rem;
    height: 30rem;
    transform-style: preserve-3d;
    transform: perspective(500px) rotateX(60deg);
  }

  .circle span {
    position: absolute;
    left: 200px;
    display: block;
    border: 3px solid var(--black);
    border-radius: 50%;
    animation: animate 3s ease-in-out infinite;
  }

  @keyframes animate {
    0%,
    100% {
      transform: translateZ(-60px);
    }
    50% {
      transform: translateZ(120px);
    }
  }

  .circle span:nth-child(1) {
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    animation-delay: 0.9s;
  }

  .circle span:nth-child(2) {
    top: 15px;
    left: 15px;
    bottom: 15px;
    right: 15px;
    animation-delay: 0.8s;
  }
  .circle span:nth-child(3) {
    top: 30px;
    left: 30px;
    bottom: 30px;
    right: 30px;
    animation-delay: 0.7s;
  }

  .circle span:nth-child(4) {
    top: 45px;
    left: 45px;
    bottom: 45px;
    right: 45px;
    animation-delay: 0.6s;
  }
  .circle span:nth-child(5) {
    top: 60px;
    left: 60px;
    bottom: 60px;
    right: 60px;
    animation-delay: 0.5s;
  }
  .circle span:nth-child(6) {
    top: 75px;
    left: 75px;
    bottom: 75px;
    right: 75px;
    animation-delay: 0.4s;
  }
  .circle span:nth-child(7) {
    top: 90px;
    left: 90px;
    bottom: 90px;
    right: 90px;
    animation-delay: 0.3s;
  }
  .circle span:nth-child(8) {
    top: 105px;
    left: 105px;
    bottom: 105px;
    right: 105px;
    animation-delay: 0.2s;
  }
  .circle span:nth-child(9) {
    top: 120px;
    left: 120px;
    bottom: 120px;
    right: 120px;
    animation-delay: 0.1s;
  }
  .circle span:nth-child(10) {
    top: 135px;
    left: 135px;
    bottom: 135px;
    right: 135px;
    animation-delay: 0s;
  }
</style>
