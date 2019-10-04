<style>
  /* ===================================================================
 * 19. footer - (_layout.scss)
 *
 * ------------------------------------------------------------------- */
  footer {
    text-align: center;
    padding-bottom: 3rem;
    position: relative;
  }

  footer a,
  footer a:visited {
    color: #ffffff;
    -moz-transition: all 0.3s ease-in-out;
    -o-transition: all 0.3s ease-in-out;
    -webkit-transition: all 0.3s ease-in-out;
    -ms-transition: all 0.3s ease-in-out;
    transition: all 0.3s ease-in-out;
  }

  footer a:hover,
  footer a:focus,
  footer a:active {
    color: #f9da4f;
    outline: 0;
  }

  .footer-social-wrap {
    background: #111;
  }

  .footer-social-list {
    list-style: none;
    display: block;
    margin: 0;
  }

  .footer-social-list li {
    display: inline-block;
    padding-left: 0;
  }

  .footer-social-list li a {
    font-size: 4.2rem;
    line-height: 4.2rem;
    color: #ffffff;
    display: block;
    padding: 4.2rem 5rem 4.8rem;
    border-right: 1px solid rgba(255, 255, 255, 0.02);
  }

  .footer-social-list li a:hover,
  .footer-social-list li a:focus,
  .footer-social-list li a:active {
    color: #f9da4f;
  }

  .footer-social-list li:first-child a {
    border-left: 1px solid rgba(255, 255, 255, 0.02);
  }

  .footer-info {
    padding-top: 6.6rem;
    padding-bottom: 6rem;
  }

  .footer-info a,
  .footer-info a:visited {
    color: #292c35;
  }

  .footer-info a:hover,
  .footer-info a:focus,
  .footer-info a:active {
    color: #ffffff;
  }

  .footer-info h4 {
    color: #ffffff;
  }

  .footer-info h4 i {
    margin-right: 10px;
    font-size: 1.2em;
    position: relative;
    top: 3px;
  }

  .footer-info .footer-link-list {
    margin: 0 0 3rem 0;
    padding: 0;
    list-style: none;
  }

  .footer-info .footer-link-list li {
    padding: 0;
  }

  .copyright span {
    display: inline-block;
  }

  .copyright span::after {
    content: "|";
    display: inline-block;
    padding: 0 1rem 0 1.2rem;
    color: rgba(255, 255, 255, 0.1);
  }

  .copyright span:last-child::after {
    display: none;
  }

  /* ------------------------------------------------------------------- 
 * responsive:
 * footer
 * ------------------------------------------------------------------- */
  @media only screen and (max-width: 1024px) {
    .footer-social-list li a {
      font-size: 3.6rem;
      line-height: 3.6rem;
      padding: 3.9rem 3rem 4.2rem;
    }
  }

  @media only screen and (max-width: 768px) {
    .footer-social-list li a {
      font-size: 3.3rem;
      line-height: 3.3rem;
      padding: 3.6rem 2rem 3.9rem;
      border: none !important;
    }
  }

  @media only screen and (max-width: 600px) {
    .footer-social-list li a {
      font-size: 3rem;
      line-height: 3rem;
      padding: 3.3rem 1.5rem 3.6rem;
      border: none;
    }

    .copyright span {
      display: block;
    }

    .copyright span::after {
      display: none;
    }
  }

  @media only screen and (max-width: 500px) {
    .footer-social-list li a {
      font-size: 2.8rem;
      line-height: 2.8rem;
      padding: 3rem 1rem 3.3rem;
      border: none;
    }
  }

  @media only screen and (max-width: 400px) {
    .footer-social-list li a {
      font-size: 2.5rem;
      line-height: 2.5rem;
      padding: 2.7rem 0.8rem 3rem;
      border: none;
    }
  }
</style>

<!-- footer
	================================================== -->
<footer id="main-footer">
  <div class="footer-social-wrap">
    <div class="row">
      <ul class="footer-social-list">
        <li>
          <a href="#facebook">
            <i class="fa fa-facebook-square" />
          </a>
        </li>
        <li>
          <a href="#twitter">
            <i class="fa fa-twitter" />
          </a>
        </li>
        <li>
          <a href="#google">
            <i class="fa fa-google-plus" />
          </a>
        </li>
        <li>
          <a href="#pinterest">
            <i class="fa fa-pinterest" />
          </a>
        </li>
        <li>
          <a href="#instagram">
            <i class="fa fa-instagram" />
          </a>
        </li>
        <li>
          <a href="#dribbble">
            <i class="fa fa-dribbble" />
          </a>
        </li>
      </ul>
    </div>
  </div>
  <!-- /footer-social-wrap -->

  <div class="footer-info-wrap">
    <div class="row footer-info">
      <div class="col-four tab-full">
        <h4>
          <i class="icon-location-map-1" />
          Where to Find Us
        </h4>

        <p>
          1600 Amphitheatre Parkway
          <br />
          Mountain View, CA
          <br />
          94043 US
        </p>
      </div>

      <div class="col-four tab-full collapse">
        <h4>
          <i class="icon-phone-incoming" />
          Get In Touch
        </h4>

        <p>
          someone@elevatewebsite.com
          <br />
          info@elevatewebsite.com
          <br />
          Phone: (+63) 555 1212
        </p>
      </div>

      <div class="col-four tab-full">
        <h4>
          <i class="icon-organization-hierarchy-3" />
          Company Links
        </h4>

        <ul class="footer-link-list">
          <li>
            <a href="#Company">Company Journal</a>
          </li>
          <li>
            <a href="#Product">Product Support</a>
          </li>
          <li>
            <a href="#Privacy">Privacy Policy</a>
          </li>
        </ul>
      </div>
    </div>
  </div>
  <!-- /footer-info-wrap -->

  <div class="footer-bottom">
    <div class="copyright">
      <span>© Copyright Elevate 2016.</span>
      <span>
        Design by
        <a href="http://www.styleshout.com/">styleshout</a>
      </span>
    </div>
  </div>
</footer>
