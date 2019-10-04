<style>
  /* ------------------------------------------------------------------- 
 * go to top - (_layout.scss)
 * ------------------------------------------------------------------- */
  #go-top {
    position: fixed;
    bottom: 0;
    right: 0;
    z-index: 800;
    display: none;
  }

  #go-top a {
    text-decoration: none;
    border: none;
    display: block;
    width: 6rem;
    height: 6.6rem;
    line-height: 6.6rem;
    text-align: center;
    background: #000000;
    color: #ffffff;
  }

  #go-top a i {
    font-size: 1.6rem;
    line-height: inherit;
  }

  #go-top a:hover,
  #go-top a:focus {
    background: #ce1137;
  }
</style>

<div id="go-top">
  <a class="smoothscroll" title="Back to Top" href="#top">
    <i class="fa fa-long-arrow-up" />
  </a>
</div>
