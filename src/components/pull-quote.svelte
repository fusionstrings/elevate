<style>
  /** 
 * Pull Quotes
 * -----------
 * markup:
 *
 * <aside>
 *		<blockquote>
 *			<p></p>
 *		</blockquote>
 *	</aside>
 *
 * --------------------------------------------------------------------- 
 */
  aside {
    position: relative;
    padding: 2.1rem 3rem 2.1rem 0px;
  }

  aside:before,
  aside:after {
    height: 1em;
    position: absolute;
    font-size: 8rem;
    font-family: Arial, Sans-Serif;
    color: rgba(17, 17, 17, 0.5);
  }

  aside:before {
    content: "\201C";
    top: 33px;
    left: 0;
  }

  aside:after {
    content: "\201D";
    bottom: -33px;
    right: 0;
  }

  aside blockquote {
    margin: 0;
  }

  aside blockquote:before {
    content: none;
  }
</style>

<aside>
  <blockquote>
    <slot />
  </blockquote>
</aside>
