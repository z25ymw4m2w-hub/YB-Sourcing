# YB-Sourcing
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>YB Sourcing | Smart Sourcing. Stronger Returns.</title>
  <meta name="description" content="YB Sourcing is a London-based property sourcing company specialising in the Rent-to-Serviced Accommodation model. Data-driven deal sourcing, analysis, and end-to-end investor support." />
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;500;600&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet" />
  <style>
    :root {
      --navy: #0A0F1E;
      --navy-mid: #0D1326;
      --navy-light: #161c30;
      --navy-border: #2a2f45;
      --gold: #C9A84C;
      --gold-light: #e2c06e;
      --gold-pale: rgba(201,168,76,0.08);
      --white: #ffffff;
      --muted: #8a8fa8;
      --muted-light: #b0b5cc;
      --font-display: 'Cormorant Garamond', serif;
      --font-body: 'DM Sans', sans-serif;
    }
 
    * { box-sizing: border-box; margin: 0; padding: 0; }
 
    html { scroll-behavior: smooth; }
 
    body {
      font-family: var(--font-body);
      background: var(--navy);
      color: var(--white);
      font-size: 15px;
      line-height: 1.7;
      overflow-x: hidden;
    }
 
    /* SCROLLBAR */
    ::-webkit-scrollbar { width: 6px; }
    ::-webkit-scrollbar-track { background: var(--navy); }
    ::-webkit-scrollbar-thumb { background: var(--navy-border); border-radius: 3px; }
 
    /* NAV */
    nav {
      position: fixed;
      top: 0; left: 0; right: 0;
      z-index: 100;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 1.25rem 3rem;
      background: rgba(10,15,30,0.92);
      backdrop-filter: blur(12px);
      border-bottom: 0.5px solid var(--navy-border);
    }
 
    .nav-logo { text-decoration: none; }
    .nav-logo-name {
      font-family: var(--font-display);
      font-size: 22px;
      font-weight: 600;
      color: var(--gold);
      letter-spacing: 0.08em;
      display: block;
      line-height: 1;
    }
    .nav-logo-tag {
      font-size: 9px;
      color: var(--muted);
      letter-spacing: 0.16em;
      text-transform: uppercase;
    }
 
    .nav-links {
      display: flex;
      gap: 2rem;
      list-style: none;
    }
    .nav-links a {
      font-size: 13px;
      color: var(--muted);
      text-decoration: none;
      letter-spacing: 0.04em;
      transition: color 0.2s;
    }
    .nav-links a:hover { color: var(--gold); }
 
    .nav-cta {
      font-family: var(--font-body);
      font-size: 13px;
      font-weight: 500;
      padding: 9px 22px;
      border-radius: 2px;
      border: 1px solid var(--gold);
      color: var(--gold);
      background: transparent;
      cursor: pointer;
      letter-spacing: 0.06em;
      text-transform: uppercase;
      transition: background 0.2s, color 0.2s;
    }
    .nav-cta:hover { background: var(--gold); color: var(--navy); }
 
    .nav-mobile-toggle { display: none; background: none; border: none; cursor: pointer; }
    .nav-mobile-toggle span { display: block; width: 22px; height: 1.5px; background: var(--gold); margin: 5px 0; }
 
    /* HERO */
    .hero {
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      padding: 8rem 2rem 5rem;
      position: relative;
      overflow: hidden;
    }
 
    .hero::before {
      content: '';
      position: absolute;
      inset: 0;
      background:
        radial-gradient(ellipse 60% 50% at 50% 80%, rgba(201,168,76,0.07) 0%, transparent 70%),
        radial-gradient(ellipse 40% 30% at 80% 20%, rgba(201,168,76,0.04) 0%, transparent 60%);
      pointer-events: none;
    }
 
    .hero-grid-bg {
      position: absolute;
      inset: 0;
      background-image:
        linear-gradient(var(--navy-border) 1px, transparent 1px),
        linear-gradient(90deg, var(--navy-border) 1px, transparent 1px);
      background-size: 60px 60px;
      opacity: 0.25;
      pointer-events: none;
    }
 
    .hero-badge {
      display: inline-flex;
      align-items: center;
      gap: 7px;
      font-size: 11px;
      padding: 5px 16px;
      border-radius: 99px;
      border: 0.5px solid var(--gold);
      color: var(--gold);
      margin-bottom: 2rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      position: relative;
    }
 
    .hero h1 {
      font-family: var(--font-display);
      font-size: clamp(42px, 7vw, 72px);
      font-weight: 500;
      line-height: 1.1;
      color: var(--white);
      margin-bottom: 1.5rem;
      position: relative;
    }
 
    .hero h1 .gold { color: var(--gold); }
 
    .hero-sub {
      font-size: 15px;
      color: var(--muted);
      max-width: 520px;
      line-height: 1.8;
      margin-bottom: 2.5rem;
      position: relative;
    }
 
    .hero-btns {
      display: flex;
      gap: 14px;
      justify-content: center;
      flex-wrap: wrap;
      position: relative;
    }
 
    .btn-gold {
      padding: 13px 30px;
      border-radius: 2px;
      background: var(--gold);
      color: var(--navy);
      border: none;
      font-family: var(--font-body);
      font-size: 13px;
      font-weight: 500;
      cursor: pointer;
      letter-spacing: 0.06em;
      text-transform: uppercase;
      text-decoration: none;
      display: inline-block;
      transition: background 0.2s;
    }
    .btn-gold:hover { background: var(--gold-light); }
 
    .btn-outline {
      padding: 13px 30px;
      border-radius: 2px;
      background: transparent;
      color: var(--gold);
      border: 1px solid var(--gold);
      font-family: var(--font-body);
      font-size: 13px;
      font-weight: 500;
      cursor: pointer;
      letter-spacing: 0.06em;
      text-transform: uppercase;
      text-decoration: none;
      display: inline-block;
      transition: background 0.2s, color 0.2s;
    }
    .btn-outline:hover { background: var(--gold-pale); }
 
    .hero-scroll {
      position: absolute;
      bottom: 2.5rem;
      left: 50%;
      transform: translateX(-50%);
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 6px;
      color: var(--muted);
      font-size: 11px;
      letter-spacing: 0.1em;
      text-transform: uppercase;
    }
    .scroll-line {
      width: 1px;
      height: 40px;
      background: linear-gradient(to bottom, var(--gold), transparent);
      animation: scrollPulse 2s ease-in-out infinite;
    }
    @keyframes scrollPulse { 0%,100% { opacity: 0.4; } 50% { opacity: 1; } }
 
    /* SECTIONS */
    section { padding: 5rem 3rem; }
    .section-inner { max-width: 1100px; margin: 0 auto; }
 
    .section-label {
      font-size: 11px;
      color: var(--gold);
      text-transform: uppercase;
      letter-spacing: 0.14em;
      margin-bottom: 0.75rem;
    }
 
    .section-title {
      font-family: var(--font-display);
      font-size: clamp(28px, 4vw, 40px);
      font-weight: 500;
      color: var(--white);
      margin-bottom: 0.75rem;
      line-height: 1.2;
    }
 
    .section-sub {
      font-size: 14px;
      color: var(--muted);
      max-width: 520px;
      line-height: 1.8;
      margin-bottom: 3rem;
    }
 
    .divider { height: 0.5px; background: var(--navy-border); margin: 0 3rem; }
 
    /* PRODUCTS */
    .products {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 1px;
      background: var(--navy-border);
      border: 0.5px solid var(--navy-border);
    }
 
    .product-card {
      background: var(--navy-mid);
      padding: 2.5rem 2rem;
      position: relative;
      transition: background 0.2s;
    }
    .product-card:hover { background: var(--navy-light); }
    .product-card.featured { background: var(--navy-light); }
 
    .product-card.featured::before {
      content: 'Most popular';
      position: absolute;
      top: 0; left: 2rem;
      font-size: 10px;
      padding: 4px 12px;
      background: var(--gold);
      color: var(--navy);
      font-weight: 500;
      letter-spacing: 0.06em;
      text-transform: uppercase;
    }
 
    .product-icon {
      width: 44px; height: 44px;
      border: 0.5px solid var(--gold);
      display: flex; align-items: center; justify-content: center;
      margin-bottom: 1.5rem;
      color: var(--gold);
      font-size: 20px;
    }
 
    .product-tag {
      font-size: 10px;
      color: var(--gold);
      text-transform: uppercase;
      letter-spacing: 0.1em;
      margin-bottom: 0.4rem;
    }
 
    .product-name {
      font-family: var(--font-display);
      font-size: 22px;
      font-weight: 500;
      color: var(--white);
      margin-bottom: 0.5rem;
    }
 
    .product-desc {
      font-size: 13px;
      color: var(--muted);
      line-height: 1.7;
      margin-bottom: 1.5rem;
    }
 
    .product-list { list-style: none; display: flex; flex-direction: column; gap: 10px; }
    .product-list li {
      font-size: 13px;
      color: var(--muted-light);
      display: flex;
      align-items: flex-start;
      gap: 10px;
    }
    .product-list li::before {
      content: '—';
      color: var(--gold);
      flex-shrink: 0;
      font-size: 12px;
      margin-top: 2px;
    }
 
    /* STEPS */
    .steps { display: flex; flex-direction: column; gap: 0; }
    .step {
      display: flex;
      gap: 2rem;
      align-items: flex-start;
      padding: 2rem 0;
      border-bottom: 0.5px solid var(--navy-border);
    }
    .step:last-child { border-bottom: none; }
 
    .step-num {
      font-family: var(--font-display);
      font-size: 48px;
      font-weight: 400;
      color: var(--navy-border);
      line-height: 1;
      min-width: 60px;
      transition: color 0.2s;
    }
    .step:hover .step-num { color: var(--gold); }
 
    .step-title {
      font-family: var(--font-display);
      font-size: 22px;
      font-weight: 500;
      color: var(--white);
      margin-bottom: 0.4rem;
    }
 
    .step-desc { font-size: 13px; color: var(--muted); line-height: 1.7; }
 
 
    /* FAQ */
    .faq { display: flex; flex-direction: column; }
    .faq-item {
      border-bottom: 0.5px solid var(--navy-border);
      overflow: hidden;
    }
 
    .faq-q {
      font-size: 14px;
      font-weight: 500;
      color: var(--white);
      padding: 1.25rem 0;
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 1rem;
      cursor: pointer;
      user-select: none;
      transition: color 0.2s;
    }
    .faq-q:hover { color: var(--gold); }
 
    .faq-icon {
      color: var(--gold);
      font-size: 18px;
      flex-shrink: 0;
      transition: transform 0.3s;
    }
    .faq-item.open .faq-icon { transform: rotate(45deg); }
 
    .faq-a {
      font-size: 13px;
      color: var(--muted);
      line-height: 1.8;
      max-height: 0;
      overflow: hidden;
      transition: max-height 0.35s ease, padding 0.3s;
      padding-bottom: 0;
    }
    .faq-item.open .faq-a { max-height: 200px; padding-bottom: 1.25rem; }
 
    /* ABOUT */
    .about-grid {
      display: grid;
      grid-template-columns: 1fr 2fr;
      gap: 4rem;
      align-items: center;
    }
 
    .about-left { position: relative; }
 
    .about-monogram {
      width: 100%;
      aspect-ratio: 1;
      max-width: 280px;
      border: 0.5px solid var(--navy-border);
      display: flex;
      align-items: center;
      justify-content: center;
      background: var(--navy-mid);
      position: relative;
    }
    .about-monogram::before {
      content: '';
      position: absolute;
      top: 12px; left: 12px; right: -12px; bottom: -12px;
      border: 0.5px solid var(--gold);
      opacity: 0.3;
      pointer-events: none;
    }
    .about-monogram-text {
      font-family: var(--font-display);
      font-size: 80px;
      font-weight: 600;
      color: var(--gold);
      letter-spacing: -2px;
      opacity: 0.6;
    }
 
    .about-role {
      font-size: 11px;
      color: var(--gold);
      text-transform: uppercase;
      letter-spacing: 0.12em;
      margin-bottom: 1rem;
    }
    .about-name {
      font-family: var(--font-display);
      font-size: 32px;
      font-weight: 500;
      color: var(--white);
      margin-bottom: 1.5rem;
    }
    .about-bio {
      font-size: 14px;
      color: var(--muted);
      line-height: 1.9;
    }
    .about-bio .highlight { color: var(--muted-light); }
 
    /* NEWSLETTER */
    .newsletter-section {
      background: var(--navy-mid);
      border-top: 1px solid var(--gold);
      border-bottom: 0.5px solid var(--navy-border);
    }
 
    .newsletter-inner {
      max-width: 600px;
      margin: 0 auto;
      text-align: center;
    }
 
    .newsletter-inner .section-title { margin-bottom: 0.5rem; }
    .newsletter-inner .section-sub { margin: 0 auto 2rem; }
 
    .newsletter-form {
      display: flex;
      gap: 0;
      max-width: 440px;
      margin: 0 auto;
    }
 
    .newsletter-form input {
      flex: 1;
      font-family: var(--font-body);
      font-size: 13px;
      padding: 12px 16px;
      border: 0.5px solid var(--navy-border);
      border-right: none;
      background: var(--navy-light);
      color: var(--white);
      outline: none;
    }
    .newsletter-form input::placeholder { color: var(--muted); }
    .newsletter-form input:focus { border-color: var(--gold); }
 
    .newsletter-form button {
      font-family: var(--font-body);
      font-size: 13px;
      font-weight: 500;
      padding: 12px 22px;
      background: var(--gold);
      color: var(--navy);
      border: none;
      cursor: pointer;
      letter-spacing: 0.06em;
      text-transform: uppercase;
      white-space: nowrap;
      transition: background 0.2s;
    }
    .newsletter-form button:hover { background: var(--gold-light); }
 
    /* LANDLORDS */
    .landlord-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 4rem;
      align-items: start;
    }
 
    .landlord-text {
      font-size: 14px;
      color: var(--muted);
      line-height: 1.9;
      margin-bottom: 1.25rem;
    }
 
    .landlord-cta-group {
      display: flex;
      gap: 12px;
      flex-wrap: wrap;
      margin-top: 2rem;
    }
 
    .landlord-benefits {
      display: flex;
      flex-direction: column;
      gap: 0;
    }
 
    .benefit-item {
      display: flex;
      gap: 1.25rem;
      align-items: flex-start;
      padding: 1.25rem 0;
      border-bottom: 0.5px solid var(--navy-border);
    }
    .benefit-item:first-child { border-top: 0.5px solid var(--navy-border); }
 
    .benefit-icon {
      width: 28px;
      height: 28px;
      border: 0.5px solid var(--gold);
      color: var(--gold);
      font-size: 13px;
      display: flex;
      align-items: center;
      justify-content: center;
      flex-shrink: 0;
      margin-top: 2px;
    }
 
    .benefit-title {
      font-size: 14px;
      font-weight: 500;
      color: var(--white);
      margin-bottom: 3px;
    }
 
    .benefit-desc {
      font-size: 12px;
      color: var(--muted);
      line-height: 1.7;
    }
 
    @media (max-width: 768px) {
      .landlord-grid { grid-template-columns: 1fr; gap: 2.5rem; }
    }
 
    /* FOOTER */
    footer {
      padding: 2.5rem 3rem;
      background: var(--navy-mid);
      border-top: 0.5px solid var(--navy-border);
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
      gap: 1.5rem;
    }
 
    .footer-brand .name {
      font-family: var(--font-display);
      font-size: 20px;
      color: var(--gold);
      letter-spacing: 0.06em;
      margin-bottom: 2px;
    }
    .footer-brand .legal { font-size: 11px; color: var(--muted); }
 
    .footer-contact { text-align: center; }
    .footer-contact a {
      display: block;
      font-size: 12px;
      color: var(--muted);
      text-decoration: none;
      transition: color 0.2s;
    }
    .footer-contact a:hover { color: var(--gold); }
 
    .footer-links { display: flex; gap: 1.5rem; }
    .footer-links a {
      font-size: 12px;
      color: var(--muted);
      text-decoration: none;
      letter-spacing: 0.05em;
      transition: color 0.2s;
    }
    .footer-links a:hover { color: var(--gold); }
 
    .footer-bottom {
      border-top: 0.5px solid var(--navy-border);
      padding: 1rem 3rem;
      text-align: center;
      font-size: 11px;
      color: var(--muted);
    }
 
    /* MOBILE */
    @media (max-width: 768px) {
      nav { padding: 1rem 1.5rem; }
      .nav-links, .nav-cta { display: none; }
      .nav-mobile-toggle { display: block; }
      section { padding: 3.5rem 1.5rem; }
      .divider { margin: 0 1.5rem; }
      .about-grid { grid-template-columns: 1fr; gap: 2rem; }
      .about-monogram { max-width: 180px; }
      footer { padding: 2rem 1.5rem; flex-direction: column; text-align: center; }
      .footer-contact { order: -1; }
      .newsletter-form { flex-direction: column; }
      .newsletter-form input { border-right: 0.5px solid var(--navy-border); border-bottom: none; }
      .footer-bottom { padding: 1rem 1.5rem; }
    }
  </style>
</head>
<body>
 
  <!-- NAV -->
  <nav>
    <a href="#" class="nav-logo">
      <span class="nav-logo-name">YB SOURCING</span>
      <span class="nav-logo-tag">Smart Sourcing. Stronger Returns.</span>
    </a>
    <ul class="nav-links">
      <li><a href="#services">Services</a></li>
      <li><a href="#process">How it works</a></li>
      <li><a href="#faq">FAQ</a></li>
      <li><a href="#landlords">Landlords</a></li>
      <li><a href="#about">About</a></li>
    </ul>
    <button class="nav-cta" onclick="document.getElementById('contact').scrollIntoView({behavior:'smooth'})">Book a call</button>
    <button class="nav-mobile-toggle" aria-label="Menu">
      <span></span><span></span><span></span>
    </button>
  </nav>
 
  <!-- HERO -->
  <section class="hero" id="home">
    <div class="hero-grid-bg"></div>
    <div class="hero-badge">&#9679; London R2SA Specialists</div>
    <h1>We Source.<br><span class="gold">You Succeed.</span></h1>
    <p class="hero-sub">YB Sourcing guides investors through the entire rent-to-serviced accommodation journey — from finding your area and building your brand, to securing a deal and connecting you with expert consultants.</p>
    <div class="hero-btns">
      <a href="#services" class="btn-gold">View our services</a>
      <a href="https://www.youtube.com/@YBSourcing" target="_blank" rel="noopener" class="btn-outline">Watch our videos</a>
    </div>
    <div class="hero-scroll">
      <div class="scroll-line"></div>
      <span>Scroll</span>
    </div>
  </section>
 
  <!-- SERVICES -->
  <section id="services">
    <div class="section-inner">
      <div class="section-label">Our services</div>
      <div class="section-title">Three ways we can help you</div>
      <div class="section-sub">Whether you are just starting out or ready to analyse your next deal, we have the right product for your stage.</div>
      <div class="products">
        <div class="product-card featured">
          <div class="product-icon">&#9634;</div>
          <div class="product-tag">Product A</div>
          <div class="product-name">The full bundle</div>
          <div class="product-desc">Complete end-to-end support through the entire R2SA process — from strategy to securing your first deal.</div>
          <ul class="product-list">
            <li>Area research &amp; data-led strategy</li>
            <li>Website creation for your brand</li>
            <li>Deal sourcing</li>
            <li>Handoff to a qualified consultant</li>
          </ul>
        </div>
        <div class="product-card">
          <div class="product-icon">&#8962;</div>
          <div class="product-tag">Product B</div>
          <div class="product-name">Deal sourcing</div>
          <div class="product-desc">We find and deliver a verified R2SA deal in the London market — straightforward and data-backed.</div>
          <ul class="product-list">
            <li>Targeted London deal search</li>
            <li>Fully vetted opportunities</li>
            <li>R2SA model focused</li>
          </ul>
        </div>
        <div class="product-card">
          <div class="product-icon">&#9650;</div>
          <div class="product-tag">Product C</div>
          <div class="product-name">Deal analysis</div>
          <div class="product-desc">Already have a deal? We run the full numbers so you invest with confidence, not guesswork.</div>
          <ul class="product-list">
            <li>Full financial breakdown</li>
            <li>Occupancy &amp; cashflow projections</li>
            <li>Risk assessment &amp; recommendation</li>
          </ul>
        </div>
      </div>
    </div>
  </section>
 
  <div class="divider"></div>
 
  <!-- PROCESS -->
  <section id="process">
    <div class="section-inner">
      <div class="section-label">The process</div>
      <div class="section-title">Your journey with YB Sourcing</div>
      <div class="section-sub">A clear, guided process from your first conversation to your first deal.</div>
      <div class="steps">
        <div class="step">
          <div class="step-num">01</div>
          <div>
            <div class="step-title">Book a free discovery call</div>
            <div class="step-desc">We learn about your goals, budget, and where you are in your journey. No obligation, no jargon — just an honest conversation.</div>
          </div>
        </div>
        <div class="step">
          <div class="step-num">02</div>
          <div>
            <div class="step-title">Choose your product</div>
            <div class="step-desc">Based on your situation, we recommend the right service. We will never push you towards something that does not fit your stage.</div>
          </div>
        </div>
        <div class="step">
          <div class="step-num">03</div>
          <div>
            <div class="step-title">We get to work</div>
            <div class="step-desc">Area research, deal sourcing, or analysis — handled with rigour. Every recommendation is backed by real market data.</div>
          </div>
        </div>
        <div class="step">
          <div class="step-num">04</div>
          <div>
            <div class="step-title">Handoff &amp; beyond</div>
            <div class="step-desc">We connect you with a qualified consultant and stay in your corner through every stage of the process.</div>
          </div>
        </div>
      </div>
    </div>
  </section>
 
  <div class="divider"></div>
 
  <!-- FAQ -->
  <section id="faq">
    <div class="section-inner">
      <div class="section-label">Common questions</div>
      <div class="section-title">FAQ</div>
      <div class="section-sub">New to R2SA? Here are the questions we get asked most.</div>
      <div class="faq">
        <div class="faq-item">
          <div class="faq-q" onclick="toggleFaq(this)">What is the Rent to Serviced Accommodation model? <span class="faq-icon">+</span></div>
          <div class="faq-a">R2SA is a strategy where you rent a property from a landlord and sublet it as short-term serviced accommodation — similar to Airbnb — generating significantly higher returns than a standard long-term tenancy.</div>
        </div>
        <div class="faq-item">
          <div class="faq-q" onclick="toggleFaq(this)">Do I need experience to get started? <span class="faq-icon">+</span></div>
          <div class="faq-a">Not at all. Our Full Bundle is specifically designed for investors who are brand new to R2SA. We guide you through every step from area selection to deal completion.</div>
        </div>
        <div class="faq-item">
          <div class="faq-q" onclick="toggleFaq(this)">Why London specifically? <span class="faq-icon">+</span></div>
          <div class="faq-a">London has one of the highest demands for short-term serviced accommodation in the world. The data consistently supports it as one of the strongest markets for the R2SA model — higher nightly rates, stronger occupancy, and significant corporate demand.</div>
        </div>
        <div class="faq-item">
          <div class="faq-q" onclick="toggleFaq(this)">How long does the sourcing process take? <span class="faq-icon">+</span></div>
          <div class="faq-a">Timelines vary depending on your criteria and the product you choose. We will always give you a realistic, data-informed timeline during your discovery call — no vague promises.</div>
        </div>
        <div class="faq-item">
          <div class="faq-q" onclick="toggleFaq(this)">What makes YB Sourcing different? <span class="faq-icon">+</span></div>
          <div class="faq-a">We are data-driven at every stage. Before any deal reaches you, we run the full numbers — occupancy rates, nightly averages, local supply, projected cashflow, and downside scenarios. We show you the spreadsheet, not just the dream.</div>
        </div>
      </div>
    </div>
  </section>
 
  <div class="divider"></div>
 
  <!-- ABOUT -->
  <section id="about">
    <div class="section-inner">
      <div class="section-label">Who we are</div>
      <div class="about-grid">
        <div class="about-left">
          <div class="about-monogram">
            <div class="about-monogram-text">YB</div>
          </div>
        </div>
        <div class="about-right">
          <div class="about-role">Founder · London R2SA Specialist</div>
          <div class="about-name">YB Sourcing</div>
          <div class="about-bio">
            I built YB Sourcing because I know what it costs to make an uninformed decision in property. Before any deal reaches a client, I run the numbers — occupancy rates, nightly averages, local supply, projected cashflow, and downside scenarios. That rigour is what separates smart sourcing from lucky sourcing.
            <br /><br />
            Whether you are completely new to property or ready to scale, I work through the numbers with you, not just the hype. My goal is simple: to give every type of investor the clarity, strategy, and deals they need to build a profitable R2SA portfolio in London.
            <br /><br />
            If you want someone who will show you the spreadsheet, not just the dream — you are in the right place.
          </div>
        </div>
      </div>
    </div>
  </section>
 
  <div class="divider"></div>
 
  <!-- LANDLORDS -->
  <section id="landlords">
    <div class="section-inner">
      <div class="section-label">For landlords</div>
      <div class="section-title">A better way to let your property</div>
      <div class="section-sub">We offer London landlords a reliable, professional alternative to traditional lettings — guaranteed rent, no voids, and no hassle.</div>
 
      <div class="landlord-grid">
        <div class="landlord-intro">
          <p class="landlord-text">At YB Sourcing, we take on your property on a guaranteed rent basis and manage it as serviced accommodation. You receive consistent, reliable income every month — without the stress of tenants, void periods, or maintenance calls.</p>
          <p class="landlord-text">We treat every property as if it were our own. Our approach is professional, transparent, and built on long-term relationships — not short-term gains.</p>
          <div class="landlord-cta-group">
            <a href="mailto:Yuialbereketab@ybsourcing.co.uk" class="btn-gold">Get in touch</a>
            <a href="tel:07774952692" class="btn-outline">Call us</a>
          </div>
        </div>
 
        <div class="landlord-benefits">
          <div class="benefit-item">
            <div class="benefit-icon">&#10003;</div>
            <div>
              <div class="benefit-title">Guaranteed rent — paid on time, every time</div>
              <div class="benefit-desc">You receive your agreed rent regardless of occupancy. No chasing payments, no uncertainty.</div>
            </div>
          </div>
          <div class="benefit-item">
            <div class="benefit-icon">&#10003;</div>
            <div>
              <div class="benefit-title">No void periods</div>
              <div class="benefit-desc">We cover the rent whether the property is occupied or not. Your income never stops.</div>
            </div>
          </div>
          <div class="benefit-item">
            <div class="benefit-icon">&#10003;</div>
            <div>
              <div class="benefit-title">Professional property management</div>
              <div class="benefit-desc">Your property is maintained to a high standard. We handle everything so you don't have to.</div>
            </div>
          </div>
          <div class="benefit-item">
            <div class="benefit-icon">&#10003;</div>
            <div>
              <div class="benefit-title">Long-term agreements</div>
              <div class="benefit-desc">Stable, predictable income for years — not months. We are here for the long term.</div>
            </div>
          </div>
          <div class="benefit-item">
            <div class="benefit-icon">&#10003;</div>
            <div>
              <div class="benefit-title">No tenant issues</div>
              <div class="benefit-desc">We deal with everything. You simply receive your rent and enjoy peace of mind.</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
 
  <!-- NEWSLETTER -->
  <section class="newsletter-section" id="contact">
    <div class="section-inner newsletter-inner">
      <div class="section-label" style="text-align:center;">Weekly newsletter</div>
      <div class="section-title">Stay ahead of the market</div>
      <div class="section-sub">Market insights, deal breakdowns, and R2SA tips — every week, straight to your inbox. No fluff, just the numbers.</div>
      <div class="newsletter-form">
        <input type="email" placeholder="your@email.com" aria-label="Email address" />
        <button type="button">Subscribe</button>
      </div>
    </div>
  </section>
 
  <!-- FOOTER -->
  <footer>
    <div class="footer-brand">
      <div class="name">YB SOURCING</div>
      <div class="legal">YB Property Sourcing Limited</div>
    </div>
    <div class="footer-contact">
      <a href="tel:07774952692">07774 952 692</a>
      <a href="mailto:Yuialbereketab@ybsourcing.co.uk">Yuialbereketab@ybsourcing.co.uk</a>
    </div>
    <div class="footer-links">
      <a href="https://www.youtube.com/@YBSourcing" target="_blank" rel="noopener">YouTube</a>
      <a href="#">Instagram</a>
      <a href="#">Privacy</a>
    </div>
  </footer>
  <div class="footer-bottom">
    &copy; 2025 YB Property Sourcing Limited. All rights reserved.
  </div>
 
  <script>
    function toggleFaq(el) {
      const item = el.parentElement;
      const isOpen = item.classList.contains('open');
      document.querySelectorAll('.faq-item').forEach(i => i.classList.remove('open'));
      if (!isOpen) item.classList.add('open');
    }
 
    const nav = document.querySelector('nav');
    window.addEventListener('scroll', () => {
      nav.style.borderBottomColor = window.scrollY > 50 ? 'rgba(201,168,76,0.2)' : 'var(--navy-border)';
    });
  </script>
 
</body>
</html>

