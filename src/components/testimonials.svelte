<style>
  /* ===================================================================
 * 16. testimonials - (_layout.scss)
 *
 * ------------------------------------------------------------------- */
  #testimonials {
    padding: 12rem 0 10.2rem;
    background: #ffffff;
    text-align: center;
  }

  #testimonials h2 {
    margin-bottom: 3.6rem;
    padding-bottom: 3.6rem;
    position: relative;
  }

  #testimonials h2::after {
    display: block;
    background-color: rgba(0, 24, 53, 0.4);
    width: 120px;
    height: 3px;
    content: "\0020";
    position: absolute;
    left: 50%;
    bottom: 0;
    margin-left: -60px;
  }

  #testimonials .slides li p {
    font-family: var(--font-family-domine);
    font-size: 3rem;
    line-height: 1.6;
  }

  #testimonials .slides li .author-info {
    font-size: 1.6rem;
    font-weight: var(--font-weight-black);
    font-style: normal;
    text-transform: uppercase;
    letter-spacing: 0.2rem;
  }

  #testimonials .flexslider-controls {
    margin-top: 3rem;
  }

  #testimonials .flexslider-controls .flex-control-nav {
    list-style: none;
    margin: 0;
    z-index: 700;
    position: relative;
  }

  #testimonials .flexslider-controls .flex-control-nav li {
    cursor: pointer;
    display: inline-block;
    margin: 0 5px;
    padding-left: 0;
  }

  #testimonials .flexslider-controls .flex-control-nav li img {
    cursor: pointer;
    width: 60px;
    opacity: 0.3;
    border-radius: 50%;
    -moz-transition: all 0.5s ease-in-out;
    -o-transition: all 0.5s ease-in-out;
    -webkit-transition: all 0.5s ease-in-out;
    -ms-transition: all 0.5s ease-in-out;
    transition: all 0.5s ease-in-out;
  }

  #testimonials .flexslider-controls .flex-control-nav li.flex-active img {
    opacity: 1;
  }

  #testimonials .flexslider-controls .flex-control-nav li:hover img {
    opacity: 1;
  }

  /* ------------------------------------------------------------------- 
 * responsive:
 * testimonials 
 * ------------------------------------------------------------------- */
  @media only screen and (max-width: 768px) {
    #testimonials .slides li p {
      font-size: 2.8rem;
      line-height: 1.68;
    }
  }

  @media only screen and (max-width: 600px) {
    #testimonials h2 {
      font-size: 2.8rem;
      line-height: 1.393;
    }

    #testimonials .slides li p {
      font-size: 2.5rem;
      line-height: 1.615;
    }
  }

  @media only screen and (max-width: 400px) {
    #testimonials .slides li p {
      font-size: 2.2rem;
      line-height: 1.636;
    }
  }
</style>

<!-- testimonials
   	================================================== -->
<section id="testimonials">
  <div class="row testimonial-content">
    <div class="col-twelve">
      <h2 class="h01 animate-this">Hear What Our Customers Say.</h2>

      <div id="testimonial-slider" class="flexslider animate-this">
        <ul class="slides">
          <li>
            <p>
              &ldquo;Your work is going to fill a large part of your life, and
              the only way to be truly satisfied is to do what you believe is
              great work. And the only way to do great work is to love what you
              do. If you haven't found it yet, keep looking. Don't settle. As
              with all matters of the heart, you'll know when you find
              it.&rdquo;
            </p>
            <p class="author-info">&mdash; Steve Jobs</p>
          </li>
          <li>
            <p>
              &ldquo;Good design is as little design as possible. Less, but
              better - because it concentrates on the essential aspects, and the
              products are not burdened with non-essentials. Back to purity,
              back to simplicity..&rdquo;
            </p>
            <p class="author-info">&mdash; Dieter Rams</p>
          </li>
          <li>
            <p>
              &ldquo;A fundamental part of that is making mistakes together.
              There's no learning without trying lots of ideas and failing lots
              of times.&rdquo;
            </p>
            <p class="author-info">&mdash; Jony Ive</p>
          </li>
        </ul>
      </div>

      <div class="flexslider-controls animate-this">
        <ul class="flex-control-nav">
          <li>
            <img src="images/customer01.jpg" alt="" />
          </li>
          <li>
            <img src="images/customer02.jpg" alt="" />
          </li>
          <li>
            <img src="images/customer03.jpg" alt="" />
          </li>
        </ul>
      </div>
    </div>
  </div>
</section>
<!-- /testimonials -->
