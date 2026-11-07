# rong-and-roop
Official website of Rong &amp; Roop — handcrafted South Asian clothing, makeup and hairstyling.

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Rong & Roop — handcrafted South Asian clothing, makeup and hairstyling. Crafted with Culture, Styled with Love.">
  <meta name="theme-color" content="#f5eee5">
  <title>Rong & Roop | Crafted with Culture, Styled with Love</title>

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&family=Playfair+Display:wght@400;500;600;700&display=swap" rel="stylesheet">

  <style>
    :root {
      --cream: #f5eee5;
      --ivory: #fffdf9;
      --rose: #b47c72;
      --brown: #704d46;
      --dark: #382c29;
      --gold: #b89a64;
      --muted: #806f65;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: 'DM Sans', sans-serif;
      color: var(--dark);
      background: var(--ivory);
      line-height: 1.7;
    }

    a {
      text-decoration: none;
      color: inherit;
    }

    img {
      display: block;
      width: 100%;
      object-fit: cover;
    }

    .announcement {
      background: var(--brown);
      color: white;
      text-align: center;
      padding: 9px 15px;
      font-size: 11px;
      letter-spacing: 2px;
    }

    header {
      background: var(--ivory);
      padding: 18px 7%;
      display: flex;
      align-items: center;
      justify-content: space-between;
      border-bottom: 1px solid #eee4d9;
      position: sticky;
      top: 0;
      z-index: 10;
    }

    .logo {
      font-family: 'Playfair Display', serif;
      font-size: 29px;
      font-weight: 600;
      letter-spacing: 2px;
      color: var(--brown);
    }

    .logo span {
      color: var(--rose);
    }

    nav {
      display: flex;
      align-items: center;
      gap: 30px;
    }

    nav a {
      font-size: 12px;
      font-weight: 600;
      letter-spacing: 1px;
      text-transform: uppercase;
    }

    nav a:hover {
      color: var(--rose);
    }

    .nav-button {
      border: 1px solid var(--brown);
      padding: 9px 17px;
    }

    .hero {
      min-height: 590px;
      display: flex;
      align-items: center;
      padding: 70px 9%;
      background:
        linear-gradient(90deg, rgba(37,25,22,.68), rgba(37,25,22,.10)),
        url('https://images.unsplash.com/photo-1610030469983-98e550d6193c?auto=format&fit=crop&w=2000&q=85')
        center 40% / cover;
      color: white;
    }

    .hero-content {
      max-width: 580px;
    }

    .eyebrow {
      font-size: 11px;
      letter-spacing: 4px;
      text-transform: uppercase;
      margin-bottom: 20px;
    }

    .hero h1 {
      font-family: 'Playfair Display', serif;
      font-size: clamp(42px, 6vw, 76px);
      line-height: 1.12;
      font-weight: 500;
      margin-bottom: 22px;
    }

    .hero p {
      font-size: 15px;
      max-width: 440px;
      margin-bottom: 30px;
      color: #f5eee5;
    }

    .button {
      display: inline-block;
      padding: 13px 25px;
      background: var(--brown);
      color: white;
      font-size: 11px;
      letter-spacing: 1.5px;
      text-transform: uppercase;
      transition: .3s;
    }

    .button:hover {
      background: var(--rose);
      transform: translateY(-2px);
    }

    .button-light {
      background: var(--cream);
      color: var(--brown);
    }

    section {
      padding: 85px 8%;
    }

    .section-heading {
      text-align: center;
      margin-bottom: 45px;
    }

    .section-heading .eyebrow {
      color: var(--rose);
      margin-bottom: 10px;
    }

    .section-heading h2 {
      font-family: 'Playfair Display', serif;
      font-size: clamp(32px, 4vw, 45px);
      font-weight: 500;
      color: var(--brown);
    }

    .section-heading p {
      color: var(--muted);
      font-size: 14px;
      margin-top: 12px;
    }

    .intro {
      background: var(--cream);
      text-align: center;
    }

    .intro p {
      max-width: 700px;
      margin: 18px auto 0;
      color: var(--muted);
      font-size: 15px;
    }

    .categories {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 28px;
    }

    .category-card {
      position: relative;
      min-height: 440px;
      overflow: hidden;
      background: var(--cream);
    }

    .category-card img {
      height: 440px;
      transition: transform .6s;
    }

    .category-card:hover img {
      transform: scale(1.04);
    }

    .category-overlay {
      position: absolute;
      inset: 0;
      display: flex;
      flex-direction: column;
      justify-content: flex-end;
      padding: 35px;
      background: linear-gradient(transparent 35%, rgba(30,20,17,.72));
      color: white;
    }

    .category-overlay h3 {
      font-family: 'Playfair Display', serif;
      font-size: 34px;
      font-weight: 500;
      margin-bottom: 8px;
    }

    .category-overlay p {
      font-size: 13px;
      margin-bottom: 18px;
    }

    .category-overlay .button {
      width: fit-content;
    }

    .features {
      background: var(--ivory);
    }

    .feature-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 25px;
    }

    .feature-card {
      background: var(--cream);
      padding-bottom: 25px;
      text-align: center;
    }

    .feature-card img {
      height: 270px;
    }

    .feature-card h3 {
      font-family: 'Playfair Display', serif;
      color: var(--brown);
      font-size: 23px;
      font-weight: 500;
      margin: 20px 10px 5px;
    }

    .feature-card p {
      color: var(--muted);
      font-size: 13px;
      padding: 0 18px;
    }

    .feature-card a {
      display: inline-block;
      color: var(--rose);
      font-size: 11px;
      font-weight: 700;
      letter-spacing: 1px;
      margin-top: 14px;
      text-transform: uppercase;
    }

    .story {
      background: #eee2d5;
    }

    .story-layout {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 55px;
      align-items: center;
    }

    .story-image img {
      height: 460px;
    }

    .story-text .eyebrow {
      color: var(--rose);
    }

    .story-text h2 {
      font-family: 'Playfair Display', serif;
      color: var(--brown);
      font-size: 43px;
      font-weight: 500;
      line-height: 1.2;
      margin-bottom: 20px;
    }

    .story-text p {
      color: var(--muted);
      font-size: 14px;
      margin-bottom: 17px;
    }

    .contact {
      text-align: center;
      background: var(--cream);
    }

    .contact p {
      color: var(--muted);
      margin: 15px auto 25px;
      max-width: 550px;
      font-size: 14px;
    }

    .contact-links {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 12px;
    }

    footer {
      background: var(--brown);
      color: white;
      text-align: center;
      padding: 35px 20px;
    }

    footer .logo {
      color: white;
      margin-bottom: 8px;
    }

    footer p {
      color: #e9d9cf;
      font-size: 12px;
      margin-top: 8px;
    }

    footer .footer-note {
      margin-top: 22px;
      font-size: 10px;
      letter-spacing: 1px;
    }

    @media (max-width: 750px) {
      header {
        padding: 15px 5%;
        flex-wrap: wrap;
        gap: 12px;
      }

      .logo {
        font-size: 24px;
      }

      nav {
        width: 100%;
        justify-content: center;
        gap: 15px;
        flex-wrap: wrap;
      }

      nav a {
        font-size: 10px;
      }

      .nav-button {
        padding: 5px 9px;
      }

      .hero {
        min-height: 500px;
        padding: 55px 7%;
        background-position: 58% center;
      }

      section {
        padding: 65px 6%;
      }

      .categories,
      .story-layout {
        grid-template-columns: 1fr;
      }

      .category-card,
      .category-card img {
        min-height: 350px;
        height: 350px;
      }

      .feature-grid {
        grid-template-columns: 1fr;
        max-width: 450px;
        margin: auto;
      }

      .feature-card img {
        height: 300px;
      }

      .story-image img {
        height: 340px;
      }

      .story-text h2 {
        font-size: 35px;
      }
    }
  </style>
</head>

<body>

  <div class="announcement">
    CELEBRATING SOUTH ASIAN CULTURE, CRAFT & BEAUTY
  </div>

  <header>
    <a class="logo" href="#home">RONG <span>&</span> ROOP</a>

    <nav>
      <a href="#home">Home</a>
      <a href="#clothing">Clothing</a>
      <a href="#beauty">Beauty Studio</a>
      <a href="#about">Our Story</a>
      <a class="nav-button" href="#contact">Contact</a>
    </nav>
  </header>

  <main>
    <section class="hero" id="home">
      <div class="hero-content">
        <div class="eyebrow">A celebration of culture & creativity</div>
        <h1>Tradition,<br>Reimagined.</h1>
        <p>
          Discover the beauty of handcrafted South Asian fashion
          and timeless beauty experiences. Every detail tells a story.
        </p>
        <a href="#clothing" class="button button-light">Explore Our World</a>
      </div>
    </section>

    <section class="intro">
      <div class="section-heading">
        <div class="eyebrow">Welcome to Rong & Roop</div>
        <h2>Crafted with Culture,<br>Styled with Love.</h2>
      </div>
      <p>
        Rooted in South Asian traditions and inspired by modern elegance,
        Rong & Roop brings together thoughtfully crafted clothing,
        makeup artistry and hairstyling. We believe that personal style
        is a beautiful expression of identity.
      </p>
    </section>

    <section id="collections">
      <div class="section-heading">
        <div class="eyebrow">Discover Our World</div>
        <h2>Two Expressions. One Story.</h2>
        <p>Explore our clothing collections and beauty experiences.</p>
      </div>

      <div class="categories">
        <div class="category-card" id="clothing">
          <img
            src="https://images.unsplash.com/photo-1595777457583-95e059d581b8?auto=format&fit=crop&w=1000&q=85"
            alt="Fashion and clothing collection"
            loading="lazy">
          <div class="category-overlay">
            <h3>The Clothing Edit</h3>
            <p>Handcrafted pieces inspired by South Asian heritage.</p>
            <a href="#featured-clothing" class="button button-light">Explore Clothing</a>
          </div>
        </div>

        <div class="category-card" id="beauty">
          <img
            src="https://images.unsplash.com/photo-1522335789203-aabd1fc54bc9?auto=format&fit=crop&w=1000&q=85"
            alt="Makeup and beauty products"
            loading="lazy">
          <div class="category-overlay">
            <h3>The Beauty Studio</h3>
            <p>Makeup and hairstyling for your special moments.</p>
            <a href="#beauty-services" class="button button-light">Explore Beauty</a>
          </div>
        </div>
      </div>
    </section>

    <section class="features" id="featured-clothing">
      <div class="section-heading">
        <div class="eyebrow">Made with Love</div>
        <h2>Our Clothing Collection</h2>
        <p>Thoughtful designs with a touch of tradition.</p>
      </div>

      <div class="feature-grid">
        <article class="feature-card">
          <img
            src="https://images.unsplash.com/photo-1610030469983-98e550d6193c?auto=format&fit=crop&w=700&q=85"
            alt="Traditional inspired fashion"
            loading="lazy">
          <h3>Traditional Elegance</h3>
          <p>Discover timeless South Asian inspired styles.</p>
          <a href="#contact">Enquire About Products →</a>
        </article>

        <article class="feature-card">
          <img
            src="https://images.unsplash.com/photo-1483985988355-763728e1935b?auto=format&fit=crop&w=700&q=85"
            alt="Modern clothing style"
            loading="lazy">
          <h3>Modern Everyday</h3>
          <p>Comfortable designs with contemporary character.</p>
          <a href="#contact">Enquire About Products →</a>
        </article>

        <article class="feature-card">
          <img
            src="https://images.unsplash.com/photo-1490481651871-ab68de25d43d?auto=format&fit=crop&w=700&q=85"
            alt="Fashion collection"
            loading="lazy">
          <h3>Custom Creations</h3>
          <p>Explore unique pieces and personalized designs.</p>
          <a href="#contact">Request a Custom Order →</a>
        </article>
      </div>
    </section>

    <section class="features" id="beauty-services" style="background:#f5eee5;">
      <div class="section-heading">
        <div class="eyebrow">The Art of Beauty</div>
        <h2>Beauty & Styling Services</h2>
        <p>Helping you feel confident, beautiful and yourself.</p>
      </div>

      <div class="feature-grid">
        <article class="feature-card">
          <img
            src="https://images.unsplash.com/photo-1487412947147-5cebf100ffc2?auto=format&fit=crop&w=700&q=85"
            alt="Makeup beauty portrait"
            loading="lazy">
          <h3>Makeup Artistry</h3>
          <p>Personalized makeup for your special occasions.</p>
          <a href="#contact">Request a Booking →</a>
        </article>

        <article class="feature-card">
          <img
            src="https://images.unsplash.com/photo-1522337360788-8b13dee7a37e?auto=format&fit=crop&w=700&q=85"
            alt="Hairstyling inspiration"
            loading="lazy">
          <h3>Hairstyling</h3>
          <p>Beautiful hairstyles for everyday and celebrations.</p>
          <a href="#contact">Request a Booking →</a>
        </article>

        <article class="feature-card">
          <img
            src="https://images.unsplash.com/photo-1519741497674-611481863552?auto=format&fit=crop&w=700&q=85"
            alt="Wedding celebration"
            loading="lazy">
          <h3>Bridal Beauty</h3>
          <p>Special beauty experiences for your memorable day.</p>
          <a href="#contact">Request a Booking →</a>
        </article>
      </div>
    </section>

    <section class="story" id="about">
      <div class="story-layout">
        <div class="story-image">
          <img
            src="https://images.unsplash.com/photo-1539109136881-3be0616acf4b?auto=format&fit=crop&w=1000&q=85"
            alt="South Asian inspired fashion editorial"
            loading="lazy">
        </div>

        <div class="story-text">
          <div class="eyebrow">Our Philosophy</div>
          <h2>Beauty in Every Thread, Every Detail.</h2>
          <p>
            Rong & Roop is inspired by the richness of South Asian
            culture and the freedom of modern self-expression.
          </p>
          <p>
            From clothing to beauty, our vision is to celebrate
            individuality, creativity and the traditions that make
            us who we are.
          </p>
          <p>
            We believe every person deserves to feel special,
            confident and beautifully represented.
          </p>
          <a href="#contact" class="button">Connect With Us</a>
        </div>
      </div>
    </section>

    <section class="contact" id="contact">
      <div class="section-heading">
        <div class="eyebrow">Let's Connect</div>
        <h2>We Would Love to Hear From You.</h2>
      </div>

      <p>
        Interested in our clothing, a custom creation,
        makeup or hairstyling? Contact us for product enquiries
        and appointment information.
      </p>

      <div class="contact-links">
        <a href="mailto:YOUR-EMAIL@example.com" class="button">
          Email Us
        </a>
        <a href="https://instagram.com/YOUR-INSTAGRAM" class="button">
          Instagram
        </a>
      </div>
    </section>
  </main>

  <footer>
    <div class="logo">RONG & ROOP</div>
    <p>Crafted with Culture, Styled with Love.</p>
    <p>Clothing · Makeup · Hairstyling</p>
    <p class="footer-note">
      © 2026 RONG & ROOP. ALL RIGHTS RESERVED.
    </p>
  </footer>

</body>
</html>
