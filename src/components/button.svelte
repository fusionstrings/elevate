<script>
  export let href;
  export let outlined = false;
  export let primary = false;
  export let full = false;
  export let medium = false;
  export let large = false;
  export let stroke = false;
  export let type = "button";
</script>

<style>
  /* ===================================================================
 * 06. buttons - (_button-essentials.scss)
 *
 * ------------------------------------------------------------------- */

  :global(.button, a.button, button, input[type="submit"], input[type="reset"], input[type="button"]) {
    display: inline-block;
    font-weight: var(--font-weight-black);
    font-size: 1.4rem;
    text-transform: uppercase;
    letter-spacing: 0.3rem;
    height: 5.4rem;
    line-height: 5.4rem;
    padding: 0 3rem;
    margin: 0 0.3rem 1.2rem 0;
    background: #d8d8d8;
    color: #001835;
    text-decoration: none;
    cursor: pointer;
    text-align: center;
    white-space: nowrap;
    border: none;
    -moz-transition: all 0.3s ease-in-out;
    -o-transition: all 0.3s ease-in-out;
    -webkit-transition: all 0.3s ease-in-out;
    -ms-transition: all 0.3s ease-in-out;
    transition: all 0.3s ease-in-out;
  }

  :global(.button:hover, a.button:hover, button:hover, input[type="submit"]:hover, input[type="reset"]:hover, input[type="button"]:hover, .button:focus, button:focus, input[type="submit"]:focus, input[type="reset"]:focus, input[type="button"]:focus) {
    background: #bebebe;
    color: #000000;
    outline: 0;
  }
  .primary {
    background: #002f68;
    color: #ffffff;
  }
  .primary:hover,
  .primary:focus {
    background: #001835;
  }

  .full {
    width: 100%;
    margin-right: 0;
  }
  .medium {
    height: 5.7rem !important;
    line-height: 5.7rem !important;
    padding: 0 1.8rem !important;
  }
  .large {
    height: 6rem !important;
    line-height: 6rem !important;
    padding: 0rem 3rem !important;
  }

  .stroke {
    background: transparent !important;
    border: 3px solid #313131;
    line-height: 4.8rem;
  }

  .stroke.medium {
    line-height: 5.1rem !important;
  }

  .stroke.large {
    line-height: 5.4rem !important;
  }

  .stroke:hover {
    border: 3px solid #ed254d;
    color: #ed254d;
  }

  :global(button::-moz-focus-inner, input::-moz-focus-inner) {
    border: 0;
    padding: 0;
  }
  .outlined {
    border: 3px solid rgba(255, 255, 255, 0.6);
    color: white;
    margin: 0 0.9rem;
    background: transparent;
  }
  .outlined:hover,
  .outlined:focus {
    border: 3px solid #f9da4f;
    color: #f9da4f;
    background: transparent;
  }
</style>

{#if href}
  <a
    class="button"
    {href}
    class:outlined
    class:primary
    class:full
    class:medium
    class:large
    class:stroke>
    <slot />
  </a>
{:else}
  <button
    {type}
    class="button outlined"
    on:click
    class:outlined
    class:primary
    class:full
    class:medium
    class:large
    class:stroke>
    <slot />
  </button>
{/if}
