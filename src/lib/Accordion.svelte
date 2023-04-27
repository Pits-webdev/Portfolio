<script>
  export let open = false;
</script>

<div class="accordion">
  <div class="head">
    <div class="tech"><slot name="tech" /></div>
    <button on:click={() => (open = !open)}>
      {#if open}
        -
      {:else}
        +
      {/if}
    </button>
  </div>

  {#if open}
    <div class="bottom"><slot name="desc" /></div>
  {/if}

  <div class="line_hz" />
</div>

<style>
  .accordion {
    width: 100%;
    height: max-content;
    margin: 1rem 0;
    padding: 1rem 0;
  }

  .accordion:first-child {
    margin: 0 0 1rem;
  }

  .head {
    width: 100%;
    height: max-content;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  .bottom {
    width: 100%;
    height: 100%;
    margin: 1rem 0;
  }

  .line_hz {
    width: 100%;
    height: 1px;
    background-color: var(--black);
    margin: 1rem 0 0;
  }
</style>
