<script>
  export let title;
</script>

<style>
  .section-lead {
    max-width: 840px;
    margin-left: auto;
    margin-right: auto;
    text-align: center;
  }

  :global(.section-lead h2) {
    font-family: var(--font-family-domine);
    font-weight: 700;
    font-size: 4.8rem;
    line-height: 1.25;
    margin-bottom: 1.2rem;
  }

  :global(.section-lead h5) {
    color: #ed254d;
    font-size: 1.6rem;
    line-height: 1.875;
    margin-bottom: 0.3rem;
    letter-spacing: 0.4rem;
  }

  .with-bottom-line {
    position: relative;
    margin-bottom: 4.2rem;
    padding-bottom: 1.5rem;
  }

  .with-bottom-line::after {
    display: block;
    background-color: #001835;
    width: 120px;
    height: 3px;
    content: "\0020";
    position: absolute;
    left: 50%;
    bottom: 0;
    margin-left: -60px;
  }
  @media only screen and (max-width: 768px) {
    .section-lead {
      max-width: 650px;
    }

    :global(.section-lead h2) {
      font-size: 4rem;
    }
  }
  @media only screen and (max-width: 600px) {
    :global(.section-lead h2) {
      font-size: 3.3rem;
    }
  }
  @media only screen and (max-width: 400px) {
    :global(.section-lead h2) {
      font-size: 3rem;
    }
  }
</style>

<div class="section-lead">
  <div class="with-bottom-line">
    {#if title}
      <h2>{title}</h2>
    {/if}
    <slot />
  </div>
</div>
