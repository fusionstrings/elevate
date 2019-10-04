<style>
  /* ===================================================================
 * 17. download - (_layout.scss)
 *
 * ------------------------------------------------------------------- */
  #download {
    position: relative;
    background-image: url(../images/download-bg.jpg);
    background-attachment: fixed;
    background-repeat: no-repeat;
    background-position: center top;
    -webkit-background-size: cover;
    -moz-background-size: cover;
    background-size: cover;
    text-align: center;
    padding: 13.2rem 0 10.2rem;
  }

  #download .overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: #001835;
    opacity: 0.85;
  }

  #download .download-content {
    position: relative;
    max-width: 780px;
  }

  #download h2 {
    font-family: var(--font-family-domine);
    font-weight: 700;
    font-size: 4.8rem;
    line-height: 1.25;
    margin-bottom: 1.8rem;
    color: white;
  }

  #download .lead {
    color: rgba(255, 255, 255, 0.6);
  }

  #download .button {
    background: #ffffff;
    color: #001835;
    margin: 0.6rem 0 1.5rem 0;
  }

  #download .button:hover,
  #download .button:focus {
    background: #f9da4f;
  }

  /* ------------------------------------------------------------------- 
 * responsive:
 * download 
 * ------------------------------------------------------------------- */
  @media only screen and (max-width: 768px) {
    #download h2 {
      font-size: 4rem;
      line-height: 1.2;
    }
  }

  @media only screen and (max-width: 600px) {
    #download h2 {
      font-size: 3.3rem;
      line-height: 1.273;
    }

    #download .button {
      width: 100%;
    }
  }

  @media only screen and (max-width: 400px) {
    #download h2 {
      font-size: 3rem;
      line-height: 1.2;
    }
  }
</style>

<!-- download
   	================================================== -->
<section id="download">
  <div class="overlay" />

  <div class="row download-content">
    <div class="col-twelve">
      <div class="text-part">
        <h2 class="animate-this">Download Elevate Now.</h2>

        <p class="lead animate-this">
          Lorem ipsum Tempor do Excepteur nulla aute deserunt reprehenderit aute
          commodo aliquip laboris velit eu esse exercitation ex fugiat pariatur
          aute consequat. Lorem ipsum Fugiat mollit quis qui. Lorem ipsum Duis
          Excepteur Duis magna fugiat incididunt qui id quis dolor nisi irure
          proident labore ut in incididunt eiusmod est anim.
        </p>
      </div>

      <a class="button large animate-this" href="#download">Download Elevate</a>
    </div>
  </div>
</section>
<!-- /download -->
