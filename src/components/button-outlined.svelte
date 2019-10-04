<script>
  export let href;
  export let type = 'button';
</script>

<style>
  .button-outlined {
    border: 3px solid rgba(255, 255, 255, 0.6);
    color: white;
    margin: 0 0.9rem;
    background: transparent;
  }
  .button-outlined:hover,
  .button-outlined:focus {
    border: 3px solid #f9da4f;
    color: #f9da4f;
    background: transparent;
  }
</style>

{#if href}
  <a class="button button-outlined" {href}>
    <slot />
  </a>
{:else}
  <button type={type} class="button button-outlined" on:click>
    <slot />
  </button>
{/if}
