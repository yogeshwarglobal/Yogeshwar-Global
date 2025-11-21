<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>YOGESHWAR GLOBAL | Import & Export</title>
  <link href="https://fonts.googleapis.com/css?family=Montserrat:700,400&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Montserrat', Arial, sans-serif;
      background: linear-gradient(135deg, #ff9933 0%, #2ecc40 100%);
      min-height: 100vh;
      color: #333;
    }
    header {
      background: rgba(255, 153, 51, 0.95);
      color: #fff;
      box-shadow: 0 6px 20px rgba(52, 82, 53, 0.08);
      padding: 20px 0;
      position: sticky;
      top: 0;
      z-index: 10;
    }
    nav {
      display: flex;
      justify-content: center;
      gap: 36px;
    }
    nav a {
      color: #fff;
      text-decoration: none;
      font-weight: 700;
      letter-spacing: 1.5px;
      transition: color 0.2s;
    }
    nav a:hover {
      color: #2ecc40;
    }
    .brand {
      font-size: 2rem;
      font-weight: bold;
      letter-spacing: 2.5px;
      text-align: center;
      margin-bottom: 10px;
      background: linear-gradient(90deg, #ff9933 30%, #138808 70%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      text-shadow: 1px 1px 6px #c2a112;
    }
    .language-switch {
      margin-top: 10px;
      text-align: right;
      margin-right: 40px;
    }
    .language-switch button {
      background: #2ecc40;
      color: #fff;
      border: none;
      padding: 7px 18px;
      border-radius: 19px;
      font-size: 1em;
      font-weight: 500;
      cursor: pointer;
      margin-left: 16px;
      transition: background 0.2s;
    }
    .language-switch button.selected {
      background: #ff9933;
    }
    main {
      max-width: 1100px;
      margin: 30px auto 60px auto;
      padding: 24px;
      background: rgba(255,255,255,0.92);
      box-shadow: 0 10px 30px 0 rgba(44, 196, 64, 0.08);
      border-radius: 18px;
    }
    section {
      margin-bottom: 48px;
    }
    .hero {
      text-align: center;
      padding: 60px 0 35px 0;
    }
    .hero h1 {
      font-size: 3.2rem;
      font-weight: 700;
      background: linear-gradient(90deg, #ff9933 40%, #138808 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }
    .hero p {
      max-width: 600px;
      font-size: 1.35rem;
      margin: 26px auto;
      color: #333;
    }
    .services, .products, .about, .contact, .testimonials, .blog, .map {
      padding: 16px 0;
    }
    .gallery {
      display: flex;
      gap: 24px;
      flex-wrap: wrap;
      justify-content: center;
    }
    .gallery img {
      height: 140px;
      width: 220px;
      object-fit: cover;
      border-radius: 10px;
      border: 2px solid #ff9933;
      box-shadow: 0 2px 12px #13880844;
    }
    form input, form textarea {
      display: block;
      margin-bottom: 18px;
      padding: 10px;
      width: 100%;
      border-radius: 8px;
      border: 1px solid #2ecc40;
      font-size: 1em;
    }
    form button {
      background: #ff9933;
      color: #fff;
      border: none;
      padding: 12px 24px;
      border-radius: 8px;
      font-size: 1.1em;
      font-weight: bold;
      cursor: pointer;
      transition: background 0.18s;
    }
    form button:hover {
      background: #2ecc40;
    }
    footer {
      background: #138808;
      color: #fff;
      text-align: center;
      padding: 24px 0 12px 0;
      font-size: 1.1em;
      border-top: 5px solid #ff9933;
    }
    .footer-links a {
      color: #fff;
      text-decoration: underline;
      margin: 0 18px;
    }
    /* Responsive */
    @media (max-width: 700px) {
      main { padding: 9px; }
      .hero h1 { font-size: 2rem; }
      nav { gap: 18px; }
      .gallery img { width: 120px; height: 75px; }
    }
    /* Exotic pattern background splash (top-right) */
    body::after {
      content: '';
      position: fixed;
      top: 0;
      right: 0;
      width: 420px;
      height: 540px;
      background: url('https://images.unsplash.com/photo-1519125323398-675f0ddb6308?auto=format&fit=crop&w=420&q=80');
      background-size: cover;
      opacity: 0.19;
      z-index: 0;
      pointer-events: none;
      border-bottom-left-radius: 220px;
    }
  </style>
  <script>
    // Language toggle (English/Swedish)
    function setLanguage(lang) {
      document.querySelectorAll('.en').forEach(el => el.style.display = lang === 'en' ? 'block' : 'none');
      document.querySelectorAll('.sv').forEach(el => el.style.display = lang === 'sv' ? 'block' : 'none');
      document.getElementById('btn-en').classList.toggle('selected', lang === 'en');
      document.getElementById('btn-sv').classList.toggle('selected', lang === 'sv');
    }
    window.onload = function() { setLanguage('en'); }
  </script>
</head>
<body>
  <header>
    <div class="brand">YOGESHWAR GLOBAL</div>
    <nav>
      <a href="#home">Home</a>
      <a href="#about">About</a>
      <a href="#services">Services</a>
      <a href="#products">Products</a>
      <a href="#map">International Presence</a>
      <a href="#contact">Contact</a>
      <a href="#blog">Blog</a>
    </nav>
    <div class="language-switch">
      <button id="btn-en" onclick="setLanguage('en')" class="selected">English</button>
      <button id="btn-sv" onclick="setLanguage('sv')">Swedish</button>
    </div>
  </header>
  <main>
    <section class="hero" id="home">
      <div class="en">
        <h1>Connecting India & The World with Luxury Imports & Exports</h1>
        <p>Welcome to <strong>YOGESHWAR GLOBAL</strong>—your gateway to a wealth of exotic goods and business expertise. We bring you only the finest products across continents, blending the heritage of India with cutting-edge global innovation. </p>
      </div>
      <div class="sv" style="display:none;">
        <h1>[translate:Förbinder Indien och världen med exklusiv import och export]</h1>
        <p>[translate:Välkommen till YOGESHWAR GLOBAL—din port till exklusiva varor och företagsexpertis. Vi levererar endast de bästa produkterna från hela världen, där Indiens arv möter global innovation.]</p>
      </div>
    </section>
    <section class="about" id="about">
      <div class="en">
        <h2>About Us</h2>
        <p>Our story began with a vision: making luxury, quality, and authenticity accessible to every corner of the world, while promoting India’s vibrant traditions and global business acumen. Meet our world-class team and learn how we deliver excellence in every shipment.</p>
      </div>
      <div class="sv" style="display:none;">
        <h2>[translate:Om oss]</h2>
        <p>[translate:Vi startade med en vision—att göra lyx, kvalitet och äkthet tillgängligt över hela världen samtidigt som vi främjar Indiens livliga traditioner och affärskompetens. Möt vårt världsklass-team och se hur vi levererar excellens i varje leverans.]</p>
      </div>
    </section>
    <section class="services" id="services">
      <div class="en">
        <h2>Services</h2>
        <ul>
          <li>International Import/Export Consultation</li>
          <li>Sourcing rare Indian and exotic products</li>
          <li>Custom logistics solutions</li>
          <li>Compliance & customs services</li>
          <li>Trade partnerships & distribution networks</li>
        </ul>
      </div>
      <div class="sv" style="display:none;">
        <h2>[translate:Tjänster]</h2>
        <ul>
          <li>[translate:Internationell konsultation inom import/export]</li>
          <li>[translate:Inköp av sällsynta indiska och exotiska produkter]</li>
          <li>[translate:Skräddarsydda logistiklösningar]</li>
          <li>[translate:Tullhantering och lagstadgade tjänster]</li>
          <li>[translate:Handelspartnerskap och distributionsnätverk]</li>
        </ul>
      </div>
    </section>
    <section class="products" id="products">
      <div class="en">
        <h2>Product Showcase</h2>
        <div class="gallery">
          <img src="https://images.unsplash.com/photo-1542827639-5f6cadd88e8d?auto=format&w=800&q=80" alt="Saffron">
          <img src="https://images.unsplash.com/photo-1464983953574-0892a716854b?auto=format&w=800&q=80" alt="Emerald">
          <img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&w=800&q=80" alt="Jewel Artifact">
          <img src="https://images.unsplash.com/photo-1519125323398-675f0ddb6308?auto=format&w=800&q=80" alt="Royal Textile">
        </div>
      </div>
      <div class="sv" style="display:none;">
        <h2>[translate:Produkter]</h2>
        <div class="gallery">
          <img src="https://images.unsplash.com/photo-1542827639-5f6cadd88e8d?auto=format&w=800&q=80" alt="[translate:Safran]">
          <img src="https://images.unsplash.com/photo-1464983953574-0892a716854b?auto=format&w=800&q=80" alt="[translate:Smaragd]">
          <img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&w=800&q=80" alt="[translate:Juvelartefakt]">
          <img src="https://images.unsplash.com/photo-1519125323398-675f0ddb6308?auto=format&w=800&q=80" alt="[translate:Kunglig textil]">
        </div>
      </div>
    </section>
    <section class="map" id="map">
      <div class="en">
        <h2>Our International Presence</h2>
        <p>From Mumbai to Stockholm, our network connects partners, buyers, and sellers worldwide. <br><em>(Interactive map coming soon!)</em></p>
      </div>
      <div class="sv" style="display:none;">
        <h2>[translate:Vår internationella närvaro]</h2>
        <p>[translate:Från Mumbai till Stockholm, vårt nätverk kopplar samman partners, köpare och säljare över hela världen. (Interaktiv karta kommer snart!)]</p>
      </div>
    </section>
    <section class="contact" id="contact">
      <div class="en">
        <h2>Contact & Enquiry</h2>
        <form>
          <input type="text" name="name" placeholder="Your Name">
          <input type="email" name="email" placeholder="Email Address">
          <textarea name="message" rows="5" placeholder="Type your message..."></textarea>
          <button type="submit">Send Inquiry</button>
        </form>
      </div>
      <div class="sv" style="display:none;">
        <h2>[translate:Kontakt & Förfrågan]</h2>
        <form>
          <input type="text" name="name" placeholder="[translate:Ditt namn]">
          <input type="email" name="email" placeholder="[translate:E-postadress]">
          <textarea name="message" rows="5" placeholder="[translate:Skriv ditt meddelande...]"></textarea>
          <button type="submit">[translate:Skicka förfrågan]</button>
        </form>
      </div>
    </section>
    <section class="testimonials" id="testimonials">
      <div class="en">
        <h2>Testimonials</h2>
        <blockquote>
          “Yogeshwar Global helped us unlock new markets with ease and elegance. Their products are truly best-in-class.”
        </blockquote>
        <blockquote>
          “Flawless logistics and cultural understanding—an essential partner for imports from India.”
        </blockquote>
      </div>
      <div class="sv" style="display:none;">
        <h2>[translate:Omdömen]</h2>
        <blockquote>
          [translate:"Yogeshwar Global hjälpte oss att öppna nya marknader med enkelhet och elegans. Deras produkter är verkligen i toppklass."]
        </blockquote>
        <blockquote>
          [translate:"Perfekt logistik och kulturell förståelse—en ovärderlig partner för import från Indien."]
        </blockquote>
      </div>
    </section>
    <section class="blog" id="blog">
      <div class="en">
        <h2>News & Blog</h2>
        <p>Coming soon: Read our latest tips, trends, and global trade updates.</p>
      </div>
      <div class="sv" style="display:none;">
        <h2>[translate:Nyheter & Blogg]</h2>
        <p>[translate:Kommer snart: Läs våra senaste tips, trender och nyheter inom global handel.]</p>
      </div>
    </section>
  </main>
  <footer>
    <div class="footer-links">
      <a href="#home">Home</a>
      <a href="#about">About</a>
      <a href="#services">Services</a>
      <a href="#products">Products</a>
      <a href="#map">International Presence</a>
      <a href="#contact">Contact</a>
      <a href="#blog">Blog</a>
    </div>
    <div style="margin-top: 12px;">
      &copy; 2025 YOGESHWAR GLOBAL. All rights reserved. | Connect: info@yogeshwarglobal.com
    </div>
  </footer>
</body>
</html>
