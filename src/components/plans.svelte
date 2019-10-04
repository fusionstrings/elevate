<style>
  /* ===================================================================
 * 15. pricing - (_layout.scss)
 *
 * ------------------------------------------------------------------- */
  #pricing {
    background: #e2e5e7;
    padding-top: 12rem;
    padding-bottom: 9.6rem;
  }

  .pricing-content {
    margin-top: 3rem;
    max-width: 1080px;
  }

  .pricing-content .bgrid {
    margin-bottom: 3.9rem;
    padding: 0 20px;
  }

  .pricing-content .price-block {
    background-color: #ffffff;
    text-align: center;
    padding: 6rem 0 4.8rem;
    box-shadow: 0 1px 2px rgba(0, 0, 0, 0.1);
    position: relative;
  }

  .pricing-content .price-block .bottom-part {
    padding-top: 2.4rem;
    padding-left: 3rem;
    padding-right: 3rem;
  }

  .pricing-content .price-block .plan-title {
    padding-bottom: 2.4rem;
    font-size: 2.4rem;
    font-weight: var(--font-weight-bold);
    position: relative;
  }

  .pricing-content .price-block .plan-title::after {
    display: block;
    background-color: rgba(0, 24, 53, 0.3);
    width: 80px;
    height: 3px;
    content: "\0020";
    position: absolute;
    left: 50%;
    bottom: 0;
    margin-left: -40px;
  }

  .pricing-content .price-block .plan-price {
    font-family: var(--font-family-domine);
    font-weight: 700;
    color: #001835;
    font-size: 6.5rem;
    line-height: 1;
    margin-top: 4.2rem;
    margin-bottom: 0;
  }

  .pricing-content .price-block .plan-price sup {
    font-weight: var(--font-weight-black);
    font-size: 2.4rem;
    top: -3rem;
    margin-right: 3px;
  }

  .pricing-content .price-block .price-month {
    margin-bottom: 1.2rem;
    font-size: 1.8rem;
    color: #3f4452;
  }

  .pricing-content .price-block .features {
    list-style: none;
    font-size: 1.6rem;
    color: rgba(0, 0, 0, 0.5);
    margin: 0 0 4.2rem 0;
  }

  .pricing-content .price-block .features li {
    padding: 0.6rem 0;
    border-bottom: 1px solid rgba(63, 80, 96, 0.15);
  }

  .pricing-content .price-block .features li strong {
    color: #001835;
    font-weight: var(--font-weight-black);
    color: #001835;
    margin-right: 5px;
  }

  .pricing-content .price-block .features li:last-child {
    border: none;
  }

  .pricing-content .price-block .button {
    background: #002f68;
    color: #ffffff;
    padding: 0 5rem;
    margin-left: auto;
    margin-right: auto;
  }

  .pricing-content .price-block .button:hover,
  .pricing-content .price-block .button:focus {
    background: #002a5e;
    color: #ffffff;
  }

  .pricing-content .primary {
    background: #002f68;
    color: #ffffff;
  }

  .pricing-content .primary::before {
    content: attr(data-info);
    display: block;
    min-height: 48px;
    line-height: 48px;
    width: 60%;
    text-align: center;
    color: #ffffff;
    background: #ed254d;
    font-weight: var(--font-weight-black);
    font-size: 1.2rem;
    text-transform: uppercase;
    letter-spacing: 0.3rem;
    position: absolute;
    top: 0px;
    left: 50%;
    -webkit-transform: translate(-50%);
    -ms-transform: translate(-50%);
    transform: translate(-50%);
  }

  .pricing-content .primary .plan-title {
    color: #ffffff;
  }

  .pricing-content .primary .plan-title::after {
    background-color: rgba(255, 255, 255, 0.3);
  }

  .pricing-content .primary .plan-price {
    color: #ffffff;
  }

  .pricing-content .primary .price-month {
    color: rgba(255, 255, 255, 0.5);
  }

  .pricing-content .primary .button {
    background: #ffffff;
    color: #001835;
  }

  .pricing-content .primary .button:hover,
  .pricing-content .primary .button:focus {
    background: #002149;
  }

  .pricing-content .primary .features {
    color: rgba(255, 255, 255, 0.6);
  }

  .pricing-content .primary .features li {
    border-bottom: 1px solid rgba(255, 255, 255, 0.05);
  }

  .pricing-content .primary .features li strong {
    color: #ffffff;
  }

  /* ------------------------------------------------------------------- 
 * responsive:
 * pricing 
 * ------------------------------------------------------------------- */
  @media only screen and (max-width: 1024px) {
    .pricing-content {
      max-width: 650px;
    }

    .pricing-content .bgrid {
      padding: 0;
      width: 50%;
      clear: none;
    }

    .pricing-content .bgrid:nth-child(2n + 1) {
      clear: both;
    }

    .pricing-content .bgrid:last-child {
      clear: both;
      float: none;
      margin-left: auto;
      margin-right: auto;
    }
  }

  @media only screen and (max-width: 600px) {
    .pricing-content {
      max-width: 400px;
    }

    .pricing-content .bgrid {
      width: 100% !important;
      float: none !important;
      clear: both !important;
      margin-left: 0;
      margin-right: 0;
    }
  }
</style>

<!-- pricing
   	================================================== -->
<section id="pricing">
  <div class="row section-intro animate-this">
    <div class="col-twelve with-bottom-line">
      <h2>Plans and Pricing.</h2>

      <p class="lead">
        Lorem ipsum Tempor do Excepteur nulla aute deserunt reprehenderit aute
        commodo aliquip laboris velit eu esse exercitation ex fugiat pariatur
        aute consequat. Lorem ipsum Fugiat mollit quis qui. Lorem ipsum Duis
        Excepteur Duis magna fugiat incididunt qui id quis dolor nisi irure
        proident labore ut in incididunt eiusmod est anim.
      </p>
    </div>
  </div>

  <div class="row pricing-content">
    <div class="pricing-tables block-1-3 group">
      <div class="bgrid animate-this">
        <div class="price-block">
          <div class="top-part">
            <h3 class="plan-title">Starter</h3>
            <p class="plan-price">
              <sup>$</sup>
              4.99
            </p>
            <p class="price-month">Per month</p>
          </div>

          <div class="bottom-part">
            <ul class="features">
              <li>
                <strong>3GB</strong>
                Storage
              </li>
              <li>
                <strong>10GB</strong>
                Bandwidth
              </li>
              <li>
                <strong>5</strong>
                Databases
              </li>
              <li>
                <strong>30</strong>
                Email Accounts
              </li>
            </ul>

            <a class="button large" href=".">Get Started</a>
          </div>
        </div>
      </div>
      <!-- /bgrid -->

      <div class="bgrid animate-this">
        <div class="price-block primary" data-info="popular">
          <div class="top-part">
            <h3 class="plan-title">Standard</h3>
            <p class="plan-price">
              <sup>$</sup>
              9.99
            </p>
            <p class="price-month">Per month</p>
          </div>

          <div class="bottom-part">
            <ul class="features">
              <li>
                <strong>5GB</strong>
                Storage
              </li>
              <li>
                <strong>15GB</strong>
                Bandwidth
              </li>
              <li>
                <strong>7</strong>
                Databases
              </li>
              <li>
                <strong>40</strong>
                Email Accounts
              </li>
            </ul>

            <a class="button large" href=".">Get Started</a>
          </div>
        </div>
      </div>
      <!-- /bgrid -->

      <div class="bgrid animate-this">
        <div class="price-block">
          <div class="top-part">
            <h3 class="plan-title">Premium</h3>
            <p class="plan-price">
              <sup>$</sup>
              29.99
            </p>
            <p class="price-month">Per month</p>
          </div>

          <div class="bottom-part">
            <ul class="features">
              <li>
                <strong>10GB</strong>
                Storage
              </li>
              <li>
                <strong>30GB</strong>
                Bandwidth
              </li>
              <li>
                <strong>15</strong>
                Databases
              </li>
              <li>
                <strong>60</strong>
                Email Accounts
              </li>
            </ul>

            <a class="button large" href=".">Get Started</a>
          </div>
        </div>
      </div>
      <!-- /bgrid -->
    </div>
    <!-- /pricing-tables -->
  </div>
  <!-- /pricing-content -->
</section>
<!-- Pricing -->
