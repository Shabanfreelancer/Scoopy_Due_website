# Scoopy_Due_website
cd path/to/your/downloaded/site
git init
git add .
git commit -m "Initial commit"
# create a new repo on GitHub first, then:
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Scoopy — Handmade Ice Cream</title>
  <meta name="description" content="Handmade small-batch ice cream. Seasonal flavors, real ingredients." />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;800&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <header class="site-header">
    <div class="container nav">
      <a class="brand" href="#">Scoopy</a>
      <nav class="nav-links" id="navLinks">
        <a href="#flavors">Flavors</a>
        <a href="#about">About</a>
        <a href="#testimonials">Reviews</a>
        <a href="#contact" class="btn btn-small">Contact</a>
      </nav>
      <button class="hamburger" id="hamburger" aria-label="Menu" aria-expanded="false">
        <span></span><span></span><span></span>
      </button>
    </div>
  </header>

  <main>
    <section class="hero">
      <div class="container hero-grid">
        <div class="hero-copy">
          <h1>Creamy joy, <span class="highlight">one scoop</span> at a time.</h1>
          <p>Small-batch ice cream made with real fruit, local dairy, and zero shortcuts. Seasonal flavors drop every Friday.</p>
          <div class="cta-row">
            <a href="#flavors" class="btn">Shop Flavors</a>
            <a href="#about" class="btn btn-ghost">Learn More</a>
          </div>
          <div class="badges">
            <div class="badge">Handmade</div>
            <div class="badge">Local Dairy</div>
            <div class="badge">Seasonal</div>
          </div>
        </div>
        <div class="hero-media">
          <div class="hero-card">
            <div class="scoop"></div>
            <div class="hero-note">New: Mango Ripple</div>
          </div>
        </div>
      </div>
    </section>

    <section id="flavors" class="section">
      <div class="container">
        <div class="section-head">
          <h2>Weekly Flavors</h2>
          <p>Rotating menu with classics and seasonal specials.</p>
        </div>

        <div class="grid cards">
          <!-- Card -->
          <article class="card">
            <div class="card-media" style="--img:url('assets/vanilla.jpg')"></div>
            <div class="card-body">
              <h3>Madagascar Vanilla</h3>
              <p>Single-origin vanilla beans, rich and aromatic.</p>
              <div class="price-row">
                <span class="price">$6 / scoop</span>
                <button class="btn btn-small">Add</button>
              </div>
            </div>
          </article>

          <article class="card">
            <div class="card-media" style="--img:url('assets/choco.jpg')"></div>
            <div class="card-body">
              <h3>Dark Chocolate</h3>
              <p>72% cacao, deep and velvety finish.</p>
              <div class="price-row">
                <span class="price">$6 / scoop</span>
                <button class="btn btn-small">Add</button>
              </div>
            </div>
          </article>

          <article class="card">
            <div class="card-media" style="--img:url('assets/strawberry.jpg')"></div>
            <div class="card-body">
              <h3>Strawberry Fields</h3>
              <p>Ripe berries folded into creamy base.</p>
              <div class="price-row">
                <span class="price">$6 / scoop</span>
                <button class="btn btn-small">Add</button>
              </div>
            </div>
          </article>

          <article class="card">
            <div class="card-media" style="--img:url('assets/mango.jpg')"></div>
            <div class="card-body">
              <h3>Mango Ripple</h3>
              <p>Sunny mango swirls—limited seasonal drop.</p>
              <div class="price-row">
                <span class="price">$7 / scoop</span>
                <button class="btn btn-small">Add</button>
              </div>
            </div>
          </article>
        </div>
      </div>
    </section>

    <section id="about" class="section alt">
      <div class="container about-grid">
        <div>
          <h2>Our Story</h2>
          <p>We started Scoopy with a simple idea: treat ice cream like a craft. Real fruit, slow churn, and recipes we obsess over.</p>
          <ul class="checklist">
            <li>Small-batch, made daily</li>
            <li>No artificial flavors or dyes</li>
            <li>Dairy & non-dairy options</li>
          </ul>
        </div>
        <div class="about-card">
          <h3>Hours & Pickup</h3>
          <p>Mon–Sat: 11:00–20:00<br>Sun: 12:00–18:00</p>
          <p><strong>Pickup:</strong> Order online, ready in 20–30 mins.</p>
          <a href="#contact" class="btn btn-small">Contact Us</a>
        </div>
      </div>
    </section>

    <section id="testimonials" class="section">
      <div class="container">
        <div class="section-head">
          <h2>What Customers Say</h2>
        </div>
        <div class="grid testimonials">
          <figure class="quote">
            <blockquote>“Creamiest scoop in town—mango ripple is unreal.”</blockquote>
            <figcaption>— Sara A.</figcaption>
          </figure>
          <figure class="quote">
            <blockquote>“Balanced sweetness and bold flavors. Love the non-dairy options.”</blockquote>
            <figcaption>— Hamza K.</figcaption>
          </figure>
          <figure class="quote">
            <blockquote>“Fast pickup and super friendly staff.”</blockquote>
            <figcaption>— Maryam R.</figcaption>
          </figure>
        </div>
      </div>
    </section>

    <section id="contact" class="section alt">
      <div class="container contact-grid">
        <div>
          <h2>Get in Touch</h2>
          <p>Email: hello@scoopy.example<br>Phone: +92 300 0000000</p>
          <p>Visit our shop at 123 Market Street, Lahore.</p>
        </div>
        <form class="form" onsubmit="return false;">
          <label>
            <span>Name</span>
            <input type="text" placeholder="Your name" required>
          </label>
          <label>
            <span>Email</span>
            <input type="email" placeholder="you@example.com" required>
          </label>
          <label>
            <span>Message</span>
            <textarea rows="4" placeholder="How can we help?"></textarea>
          </label>
          <button class="btn">Send Message</button>
        </form>
      </div>
    </section>
  </main>

  <footer class="site-footer">
    <div class="container footer-grid">
      <div>
        <div class="brand">Scoopy</div>
        <p class="muted">© <span id="year"></span> Scoopy. All rights reserved.</p>
      </div>
      <div class="footer-links">
        <a href="#flavors">Flavors</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
        <a href="#" aria-disabled="true">Privacy</a>
      </div>
    </div>
  </footer>

  <script src="script.js"></script>
</body>
</html>
