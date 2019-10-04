<script>
  export let tabs = [];
</script>

<style>
  /** 
 * Stats Tab
 * ---------
 * markup:
 *
 * <ul class="stats-tabs">
 *		<li><a href="#">[value]<em>[name]</em></a></li>
 *	</ul>
 *
 * Extend this object into your markup.
 *
 * ---------------------------------------------------------------------
 */
  .stats-tabs {
    padding: 0;
    margin: 3rem 0;
  }

  .stats-tabs li {
    display: inline-block;
    margin: 0 1.5rem 3rem 0;
    padding: 0 1.5rem 0 0;
    border-right: 1px solid #ccc;
  }

  .stats-tabs li:last-child {
    margin: 0;
    padding: 0;
    border: none;
  }

  .stats-tabs li a {
    display: inline-block;
    font-size: 2.5rem;
    font-weight: var(--font-weight-bold);
    border: none;
    color: black;
  }

  .stats-tabs li a:hover {
    color: #ed254d;
  }

  .stats-tabs li a em {
    display: block;
    margin: 0.6rem 0 0 0;
    font-size: 1.4rem;
    color: #3f4452;
  }
</style>

<ul class="stats-tabs">
  {#each tabs as { href, name, value }}
    <li>
      {#if href}
        <a {href}>
          {value}
          {#if name}
            <em>{name}</em>
          {/if}
        </a>
      {:else}
        {value}
        {#if name}
          <em>{name}</em>
        {/if}
      {/if}
    </li>
  {/each}
</ul>
