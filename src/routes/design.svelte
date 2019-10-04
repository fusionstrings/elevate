<script>
  import HeadingHero from "../components/heading-hero.svelte";
  import SubHeadingHero from "../components/subheading-hero.svelte";
  import ButtonOutlined from "../components/button-outlined.svelte";
  import Hero from "../components/hero.svelte";
  import Footer from "../components/footer.svelte";
  import ButtonGotoTop from "../components/button-goto-top.svelte";
  import StatsTabs from "../components/stats-tabs.svelte";

  function onClick() {
    console.log("event");
  }
</script>

<style>
  .light-mode {
    background: var(--color-lightest);
  }
</style>

<HeadingHero>Hero Heading</HeadingHero>
<SubHeadingHero>Sub Heading</SubHeadingHero>
<ButtonOutlined>Outlined Button</ButtonOutlined>

<Hero
  heading="The perfect template to present your awesome product."
  subheading="Introducing Elevate"
  actions={[{ label: 'Features', href: 'features' }, { label: 'Download', onClick: onClick }]}>

  <img src="images/app-screenshot-big.jpg" alt="" class="animate-intro" />
</Hero>

<div class="light-mode">
  <div>
    <h1>This is the style page.</h1>
    <p class="lead">
      Lorem ipsum Officia elit ad tempor dolore est ex incididunt incididunt
      occaecat culpa deserunt sunt labore in cillum ullamco magna in Excepteur
      consequat in reprehenderit proident mollit incididunt officia commodo.
      Duis ea officia sed dolor pariatur enim dolore dolore quis incididunt
      nulla exercitation commodo veniam et ea incididunt.
    </p>
  </div>
  <div>
    <h3>Paragraph and Image</h3>

    <p>
      <a href="link">
        <img
          width="120"
          height="120"
          class="pull-left"
          alt="sample-image"
          src="images/sample-image.jpg" />
      </a>
      Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Donec libero.
      Suspendisse bibendum. Cras id urna. Morbi tincidunt, orci ac convallis
      aliquam, lectus turpis varius lorem, eu posuere nunc justo tempus leo.
      Donec mattis, purus nec placerat bibendum, dui pede condimentum odio, ac
      blandit ante orci ut diam. Cras fringilla magna. Phasellus suscipit, leo a
      pharetra condimentum, lorem tellus eleifend magna, eget fringilla velit
      magna id neque. posuere nunc justo tempus leo.
    </p>

    <p>
      Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Donec libero.
      Suspendisse bibendum. Cras id urna. Morbi tincidunt, orci ac convallis
      aliquam, lectus turpis varius lorem, eu posuere nunc justo tempus leo.
      Donec mattis, purus nec placerat bibendum, dui pede condimentum odio, ac
      blandit ante orci ut diam.
    </p>

    <p>
      A
      <a href="link">link</a>
      ,
      <abbr title="this really isn't a very good description">abbrebation</abbr>
      ,
      <strong>strong text</strong>
      ,
      <em>em text</em>
      ,
      <del>deleted text</del>
      , and
      <mark>this is a mark text.</mark>
      <code>.code</code>
    </p>
  </div>
  <div>
    <h3>Drop Caps</h3>

    <p class="drop-cap">
      Far far away, behind the word mountains, far from the countries Vokalia
      and Consonantia, there live the blind texts. Separated they live in
      Bookmarksgrove right at the coast of the Semantics, a large language
      ocean. A small river named Duden flows by their place and supplies it with
      the necessary regelialia. Morbi tincidunt, orci ac convallis aliquam,
      lectus turpis varius lorem, eu posuere nunc justo tempus leo. Donec
      mattis, purus nec placerat bibendum, dui pede condimentum odio, ac blandit
      ante orci ut diam. Cras fringilla magna. Phasellus suscipit, leo a
      pharetra condimentum, lorem tellus eleifend magna, eget fringilla velit
      magna id neque.
    </p>

    <h3>Small Print</h3>

    <p>
      Buy one widget, get one free!
      <small>
        (While supplies last. Offer expires on the vernal equinox. Not valid in
        Ohio.)
      </small>
    </p>
  </div>
  <div>
    <h3>Pull Quotes</h3>

    <aside class="pull-quote">
      <blockquote>
        <p>
          It is a paradisematic country, in which roasted parts of sentences fly
          into your mouth. Even the all-powerful Pointing has no control about
          the blind texts it is an almost unorthographic life One day however a
          small line of blind text by the name of Lorem Ipsum decided to leave
          for the far World of Grammar.
        </p>
      </blockquote>
    </aside>
  </div>

  <div>
    <h3>Block Quotes</h3>

    <blockquote cite="http://where-i-got-my-info-from.com">
      <p>
        Your work is going to fill a large part of your life, and the only way
        to be truly satisfied is to do what you believe is great work. And the
        only way to do great work is to love what you do. If you haven't found
        it yet, keep looking. Don't settle. As with all matters of the heart,
        you'll know when you find it.
      </p>

      <cite>
        <a href="steve-jobs">Steve Jobs</a>
      </cite>
    </blockquote>

    <blockquote>
      <p>Good design is as little design as possible.</p>
      <cite>Dieter Rams</cite>
    </blockquote>
  </div>

  <div>
    <h3>Example Lists</h3>

    <ol>
      <li>Here is an example</li>
      <li>of an ordered list.</li>
      <li>
        A parent list item.
        <ul>
          <li>one</li>
          <li>two</li>
          <li>three</li>
        </ul>
      </li>
      <li>A list item.</li>
    </ol>

    <ul class="disc">
      <li>Here is an example</li>
      <li>of an unordered list.</li>
    </ul>

    <h3>Definition Lists</h3>

    <h5>a) Multi-line Definitions (default)</h5>

    <dl>
      <dt>
        <strong>This is a term</strong>
      </dt>
      <dd>
        this is the definition of that term, which both live in a
        <code>dl</code>
        .
      </dd>
      <dt>
        <strong>Another Term</strong>
      </dt>
      <dd>And it gets a definition too, which is this line</dd>
      <dd>
        This is a 2
        <sup>nd</sup>
        definition for a single term. A
        <code>dt</code>
        may be followed by multiple
        <code>dd</code>
        s.
      </dd>
    </dl>
  </div>
  <div>
    <h3>Headers</h3>

    <h1>H1 Heading</h1>
    <h2>H2 Heading</h2>
    <h3>H3 Heading</h3>
    <h4>H4 Heading</h4>
    <h5>H5 Heading</h5>
    <h6>H6 Heading</h6>

    <h3>Buttons</h3>

    <p>
      <a class="button button-primary full-width" href="primary-button">
        Primary Button
      </a>
      <a class="button full-width" href="default-button">Default Button</a>
    </p>
  </div>

  <div>
    <h3>Stats Tabs</h3>
    <StatsTabs
      tabs={[{ href: 'stat-1', value: '1,234', name: 'Sasuke' }, { href: 'stat-2', value: '586', name: 'Hinata' }, { href: 'stat-2', value: '23,456', name: 'Naruto' }]} />

    
  </div>

  <div>
    <h3>Responsive Image</h3>

    <p>
      <img src="images/shutterbug.jpg" alt="shutterbug" />
    </p>
  </div>

  <div>
    <h3>Responsive video</h3>

    <div class="fluid-video-wrapper">
      <iframe
        title="Responsive video"
        src="http://player.vimeo.com/video/14592941?title=0&amp;byline=0&amp;portrait=0&amp;color=F64B39"
        width="500"
        height="281"
        frameborder="0"
        webkitallowfullscreen
        mozallowfullscreen
        allowfullscreen />
    </div>
  </div>

  <div>
    <h3>Tables</h3>
    <p>
      Be sure to use properly formed table markup with
      <code>&lt;thead&gt;</code>
      and
      <code>&lt;tbody&gt;</code>
      when building a
      <code>table</code>
      .
    </p>

    <div class="table-responsive">
      <table>
        <thead>
          <tr>
            <th>Name</th>
            <th>Age</th>
            <th>Sex</th>
            <th>Location</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Naruto Uzumaki</td>
            <td>16</td>
            <td>Male</td>
            <td>Konoha</td>
          </tr>
          <tr>
            <td>Sakura Haruno</td>
            <td>16</td>
            <td>Female</td>
            <td>Konoha</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</div>

<Footer />
<ButtonGotoTop />

<!-- preloader
   ================================================== -->
<div id="preloader">
  <div id="loader" />
</div>
