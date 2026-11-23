<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="A student project about nature and life.">
  <title>The Nature of Life</title>
  <style>
    /* Shared colours: edit these to change the theme. */
    :root {
      --bg: #f7f8ef;
      --green: #183f32;
      --muted: #627366;
      --border: #dee5d8;
    }
    * { box-sizing: border-box; }
    html { scroll-behavior: smooth; scroll-padding-top: 100px; }
    body {
      margin: 0;
      font-family: Arial, Helvetica, sans-serif;
      background: var(--bg);
      color: var(--green);
      line-height: 1.7;
    }
    .container { width: min(1120px, 90%); margin-inline: auto; }
    header { background: white; border-bottom: 1px solid var(--border); }
    nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 20px;
      padding: 20px 0;
    }
    .logo { font-family: Georgia, serif; font-size: 24px; font-weight: bold; }
    a { color: inherit; text-underline-offset: 5px; }
    .logo, .button { text-decoration: none; }
    .links { display: flex; gap: 20px; flex-wrap: wrap; }
    a:focus-visible { outline: 3px solid #a16622; outline-offset: 5px; }
    section { padding: 65px 0; }
    .hero { display: grid; grid-template-columns: 1fr 1fr; gap: 45px;
      align-items: center; }
    .eyebrow { font-size: 12px; letter-spacing: 2px;
      text-transform: uppercase; font-weight: bold; }
    h1, h2, h3 { font-family: Georgia, serif; line-height: 1.15; }
    h1 { font-size: clamp(48px, 6vw, 80px); margin: 15px 0 25px; }
    h2 { font-size: clamp(30px, 4vw, 44px); margin: 0 0 20px; }
    h3 { font-size: 28px; margin: 14px 0; }
    p { color: var(--muted); }
    .button { display: inline-block; padding: 12px 22px;
      background: var(--green); color: white; border-radius: 6px; }
    .button:hover { background: #397354; }
    .hero-photo { width: 100%; height: 440px; object-fit: cover;
      border-radius: 45% 45% 12px 12px; display: block; }
    .about { background: white; }
    .intro { max-width: 680px; }
    .cards { display: grid; grid-template-columns: repeat(3, 1fr); gap: 22px; }
    .card { background: white; border: 1px solid var(--border);
      border-radius: 14px; overflow: hidden;
      transition: transform 0.2s, box-shadow 0.2s; }
    .card:hover { transform: translateY(-5px);
      box-shadow: 0 14px 28px #183f3214; }
    .card img { width: 100%; height: 220px; object-fit: cover;
      object-position: center; display: block; background: #dce8cc; }
    .card-content { padding: 26px; }
    .card-content p { margin-bottom: 0; }
    .label { font-size: 12px; letter-spacing: 2px; font-weight: bold; }
    .protect { background: var(--green); color: white; }
    .protect p { color: #dce8cc; }
    ul { padding-left: 24px; }
    li { margin-bottom: 12px; }
    footer { padding: 28px 0; border-top: 1px solid var(--border); }
    footer p { margin: 0; font-size: 14px; }
    @media (max-width: 800px) {
      .hero, .cards { grid-template-columns: 1fr; }
      .hero-photo { height: 350px; }
      nav { flex-direction: column; }
      section { padding: 45px 0; }
    }
    @media (prefers-reduced-motion: reduce) {
      html { scroll-behavior: auto; }
      .card { transition: none; }
      .card:hover { transform: none; }
    }
  </style>
</head>
<body id="top">
  <header>
    <nav class="container" aria-label="Main navigation">
      <a class="logo" href="#top">NatureOfLife.</a>
      <div class="links">
        <a href="#about">About</a>
        <a href="#explore">Explore</a>
        <a href="#protect">Protect Nature</a>
      </div>
    </nav>
  </header>

  <main>
    <section class="hero container" aria-labelledby="main-title">
      <div>
        <p class="eyebrow">A student project inspired by nature</p>
        <h1 id="main-title">The Nature of Life.</h1>
        <p>Slow down, look closer, and discover the beauty of the
          living world around us.</p>
        <a class="button" href="#explore">Explore the Project</a>
      </div>
      <!-- Online photograph: an internet connection is needed. -->
      <img class="hero-photo"
        src="https://images.unsplash.com/photo-1441974231531-c6227db76b6e?auto=format&amp;fit=crop&amp;w=1200&amp;q=85"
        alt="Sunlight passing through a green forest"
        width="1200" height="800">
    </section>

    <section class="about" id="about" aria-labelledby="about-title">
      <div class="container intro">
        <p class="eyebrow">About this project</p>
        <h2 id="about-title">A closer look at our world.</h2>
        <p>This project celebrates the beauty of nature through
          forests, water, and wildlife. It invites us to observe
          our surroundings with curiosity and care.</p>
      </div>
    </section>

    <section id="explore" aria-labelledby="explore-title">
      <div class="container">
        <p class="eyebrow">Discover nature</p>
        <h2 id="explore-title">Three windows into life.</h2>
        <p class="intro">Explore real photographs of the landscapes
          and living things that inspire this project.</p>
        <div class="cards">
          <article class="card">
            <img
              src="https://images.unsplash.com/photo-1473448912268-2022ce9509d8?auto=format&amp;fit=crop&amp;w=900&amp;q=85"
              alt="Tall trees in a lush green forest"
              width="900" height="600" loading="lazy">
            <div class="card-content">
              <span class="label">01 / FORESTS</span>
              <h3>A world of green</h3>
              <p>Look beyond the trees. Notice the leaves, patterns,
                shadows, and quiet spaces that make every forest unique.</p>
            </div>
          </article>
          <article class="card">
            <img
              src="https://images.unsplash.com/photo-1518837695005-2083093ee35b?auto=format&amp;fit=crop&amp;w=900&amp;q=85"
              alt="Ocean waves beneath a bright sky"
              width="900" height="600" loading="lazy">
            <div class="card-content">
              <span class="label">02 / WATER</span>
              <h3>Life in motion</h3>
              <p>Follow the movement of a river, the rhythm of ocean
                waves, or the stillness of a pond.</p>
            </div>
          </article>
          <article class="card">
            <img
              src="https://images.unsplash.com/photo-1546182990-dffeafbe841d?auto=format&amp;fit=crop&amp;w=900&amp;q=85"
              alt="A lion resting in natural surroundings"
              width="900" height="600" loading="lazy">
            <div class="card-content">
              <span class="label">03 / WILDLIFE</span>
              <h3>Room for every life</h3>
              <p>Watch, listen, and appreciate wildlife from a respectful
                distance. Be curious without disturbing what you find.</p>
            </div>
          </article>
        </div>
      </div>
    </section>

    <section class="protect" id="protect" aria-labelledby="protect-title">
      <div class="container">
        <h2 id="protect-title">Choose care. Start close to home.</h2>
        <p>Let appreciation inspire thoughtful everyday choices.</p>
        <ul>
          <li>Notice the natural spaces around you.</li>
          <li>Treat shared outdoor places with respect.</li>
          <li>Think about what you use, keep, and throw away.</li>
          <li>Share your appreciation through art or writing.</li>
        </ul>
      </div>
    </section>
  </main>

  <footer>
    <div class="container">
      <p>The Nature of Life | Project by Your Name</p>
      <p>Photographs hosted by Unsplash. Internet connection required.</p>
      <a href="#top">Back to top</a>
    </div>
  </footer>
</body>
</html>
