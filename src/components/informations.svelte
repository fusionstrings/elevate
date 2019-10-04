<style>
  /* ===================================================================
 * 13. infos - (_layout.scss)
 *
 * ------------------------------------------------------------------- */
  #infos {
    background: #ffffff;
  }

  .info-entry {
    position: relative;
  }

  .info-entry .half-grey {
    width: 50%;
    height: 100%;
    position: absolute;
    left: 50%;
    top: 0;
    background: rgba(63, 80, 96, 0.15);
  }

  .info-entry .info-entry-content {
    position: relative;
  }

  .info-entry .media-wrap {
    width: 50%;
    position: absolute;
    top: 50%;
    -webkit-transform: translateY(-50%);
    -ms-transform: translateY(-50%);
    transform: translateY(-50%);
    z-index: 600;
  }

  .info-entry:nth-child(odd) .media-wrap {
    left: 50%;
    padding-left: 0;
    padding-right: 20px;
  }

  .info-entry:nth-child(odd) .text-part {
    padding-left: 20px;
    padding-right: 70px;
  }

  .info-entry:nth-child(even) .half-grey {
    left: 0;
  }

  .info-entry:nth-child(even) .media-wrap {
    left: 0;
    padding-right: 0;
    padding-left: 20px;
  }

  .info-entry:nth-child(even) .text-part {
    padding-left: 70px;
    padding-right: 20px;
    float: right;
  }

  .info-entry-content {
    padding-top: 13.2rem;
    padding-bottom: 10.8rem;
  }

  .info-entry-content h5 {
    color: rgba(0, 24, 53, 0.4);
    margin-bottom: 0.6rem;
    margin-left: 0.2rem;
    font-weight: var(--font-weight-medium);
    font-size: 1.5rem;
  }

  .info-entry-content h2 {
    font-family: var(--font-family-domine);
    font-weight: 700;
    font-size: 3.7rem;
    line-height: 1.216;
    padding-bottom: 1.5rem;
    position: relative;
  }

  .info-entry-content h2::after {
    content: "";
    display: block;
    width: 50px;
    height: 3px;
    background: rgba(0, 24, 53, 0.2);
    position: absolute;
    left: 0;
    bottom: 0;
  }

  .info-entry:last-child .info-entry-content {
    padding-bottom: 13.2rem;
  }

  /* ------------------------------------------------------------------- 
 * responsive:
 * infos 
 * ------------------------------------------------------------------- */
  @media only screen and (max-width: 1024px) {
    .info-entry:nth-child(odd) .media-wrap {
      padding-right: 20px;
    }

    .info-entry:nth-child(odd) .text-part {
      padding-left: 20px;
      padding-right: 40px;
    }

    .info-entry:nth-child(even) .media-wrap {
      padding-left: 20px;
    }

    .info-entry:nth-child(even) .text-part {
      padding-left: 40px;
      padding-right: 20px;
    }
  }

  @media only screen and (max-width: 900px) {
    #infos {
      padding-top: 4.2rem;
      padding-bottom: 3rem;
    }

    .info-entry .half-grey {
      display: none;
    }

    .info-entry .info-entry-content {
      max-width: 600px;
      padding-top: 9rem;
      padding-bottom: 7.8rem;
      border-bottom: 1px solid rgba(0, 24, 53, 0.1);
    }

    .info-entry .info-entry-content .media-wrap,
    .info-entry .info-entry-content .text-part {
      padding: 0 15px;
    }

    .info-entry .info-entry-content .media-wrap {
      position: static;
      width: 100%;
      -webkit-transform: translateY(0);
      -ms-transform: translateY(0);
      transform: translateY(0);
      margin-bottom: 4.2rem;
    }

    .info-entry .info-entry-content .text-part {
      width: 100% !important;
      float: none !important;
      clear: both !important;
      margin-left: 0;
      margin-right: 0;
      text-align: center;
    }

    .info-entry .info-entry-content .button {
      margin: 0 0 1.5rem 0;
    }

    .info-entry .info-entry-content h2::after {
      left: 50%;
      margin-left: -25px;
    }

    .info-entry:last-child .info-entry-content {
      border: none;
    }
  }

  @media only screen and (max-width: 600px) {
    .info-entry .info-entry-content .media-wrap,
    .info-entry .info-entry-content .text-part {
      padding: 0 10px;
    }

    .info-entry .info-entry-content h2 {
      font-size: 3rem;
      line-height: 1.3;
    }
  }

  @media only screen and (max-width: 400px) {
    .info-entry .info-entry-content {
      padding-top: 7.8rem;
      padding-bottom: 6rem;
    }

    .info-entry .info-entry-content .media-wrap,
    .info-entry .info-entry-content .text-part {
      padding: 0;
    }

    .info-entry .info-entry-content h2 {
      font-size: 2.8rem;
      line-height: 1.3;
    }
  }
</style>

<!-- infos
   	================================================== -->
<section id="infos">
  <div class="info-entry">
    <div class="half-grey" />

    <div class="row info-entry-content">
      <div class="media-wrap">
        <div class="media animate-this" data-animate="fadeInRight">
          <img src="images/app-screenshot-small.jpg" alt="" />
        </div>
      </div>

      <div class="col-six text-part">
        <h5 class="animate-this" data-animate="fadeInLeft">Some Cool Stuff</h5>
        <h2 class="animate-this" data-animate="fadeInLeft">
          Clean and Organized Code
        </h2>

        <p class="animate-this" data-animate="fadeInLeft">
          Lorem ipsum Sunt adipisicing adipisicing esse exercitation consequat
          sed irure commodo cupidatat aute ea adipisicing consectetur nulla
          consequat irure consectetur veniam sit sit qui reprehenderit officia
          sunt nulla elit nisi proident.
        </p>

        <a href="#learn" class="button animate-this" data-animate="fadeInLeft">
          Learn More
        </a>
      </div>
    </div>
    <!-- /info-entry-content -->
  </div>
  <!-- /info-entry -->

  <div class="info-entry">
    <div class="half-grey" />

    <div class="row info-entry-content">
      <div class="media-wrap">
        <div class="media animate-this" data-animate="fadeInLeft">
          <div class="fluid-video-wrapper">
            <iframe
              title="fluid-video-wrapper"
              src="http://player.vimeo.com/video/14592941?title=0&amp;byline=0&amp;portrait=0&amp;color=F64B39"
              width="500"
              height="281"
              frameborder="0"
              webkitallowfullscreen
              mozallowfullscreen
              allowfullscreen />
          </div>
        </div>
      </div>

      <div class="col-six text-part">
        <h5 class="animate-this" data-animate="fadeInRight">Video Stuff</h5>
        <h2 class="animate-this" data-animate="fadeInRight">
          Your Super Cool Video
        </h2>

        <p class="animate-this" data-animate="fadeInRight">
          Lorem ipsum Sunt adipisicing adipisicing esse exercitation consequat
          sed irure commodo cupidatat aute ea adipisicing consectetur nulla
          consequat irure consectetur veniam sit sit qui reprehenderit officia
          sunt nulla elit nisi proident.
        </p>

        <a href="#learn" class="button animate-this" data-animate="fadeInRight">
          Learn More
        </a>
      </div>
    </div>
    <!-- /info-entry-content -->
  </div>
  <!-- /info-entry -->
</section>
<!-- infos -->
