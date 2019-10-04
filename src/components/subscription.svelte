<style>
  /* ===================================================================
 * 18. subscribe - (_layout.scss)
 *
 * ------------------------------------------------------------------- */
  #subscribe {
    background: #00132b;
    padding: 10.2rem 0 6rem;
    text-align: center;
    color: #ffffff;
  }

  #subscribe .subscribe-content {
    max-width: 780px;
  }

  #subscribe #mc-form {
    margin-top: 4.2rem;
    margin-bottom: 0;
    text-align: center;
  }

  #subscribe #mc-form input[type="email"] {
    width: 100%;
    text-align: left;
    color: rgba(255, 255, 255, 0.7);
    background: rgba(0, 0, 0, 0.3);
  }

  #subscribe #mc-form input[type="email"]:focus {
    background: rgba(0, 0, 0, 0.5);
    color: white;
  }

  #subscribe #mc-form .button {
    margin: 0;
    width: 100%;
    background: #ffffff;
  }

  #subscribe #mc-form .button:hover,
  #subscribe #mc-form .button:focus {
    background: #f9da4f;
  }

  #subscribe #mc-form label {
    color: #ffffff;
  }

  #subscribe .left {
    padding-right: 0;
  }

  #subscribe .right {
    padding-left: 0;
  }

  #subscribe h2 {
    color: white;
  }

  /* ------------------------------------------------------------------- 
 * responsive:
 * subscribe 
 * ------------------------------------------------------------------- */
  @media only screen and (max-width: 768px) {
    #subscribe .subscribe-content {
      max-width: 600px;
    }

    #subscribe .left {
      padding-right: 15px;
    }

    #subscribe .right {
      padding-left: 15px;
    }

    #subscribe #mc-form input[type="email"] {
      text-align: center;
    }

    #subscribe #mc-form label {
      margin-top: 3rem;
    }
  }

  @media only screen and (max-width: 600px) {
    #subscribe h2 {
      font-size: 2.8rem;
      line-height: 1.393;
    }

    #subscribe .left {
      padding-right: 10px;
    }

    #subscribe .right {
      padding-left: 10px;
    }
  }

  @media only screen and (max-width: 400px) {
    #subscribe .left {
      padding-right: 0;
    }

    #subscribe .right {
      padding-left: 0;
    }
  }
</style>

<!-- subscribe
   	================================================== -->
<section id="subscribe">
  <div class="row subscribe-content">
    <div class="col-twelve">
      <h2 class="h01 animate-this">Stay upto date, join our newsletter</h2>
      <form id="mc-form" class="group" novalidate="true" autocomplete="off">
        <div class="row">
          <div
            class="col-eight tab-full left animate-this"
            data-animate="fadeInLeft">
            <input
              type="email"
              value=""
              name="EMAIL"
              class="email"
              id="mce-EMAIL"
              placeholder="Enter Your Email"
              required="" />
          </div>

          <div
            class="col-four tab-full right animate-this"
            data-animate="fadeInRight">
            <input
              type="submit"
              value="Get Notified"
              name="subscribe"
              class="button large" />
          </div>
        </div>
        <!-- /row -->

        <label for="mce-EMAIL" class="subscribe-message" />
      </form>
    </div>
  </div>
</section>
<!-- /subscribe -->
