<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <meta name="description" content="SEO with Tehzeeb — SEO Expert & Digital Marketing Freelancer. Helping businesses grow online with proven SEO, content marketing, and AI-powered strategies."/>
  <meta name="keywords" content="SEO with Tehzeeb, SEO expert Pakistan, digital marketing freelancer, AI marketing, content strategy, Lahore"/>
  <title>SEO with Tehzeeb — SEO & Digital Marketing Expert</title>
  <link href="https://fonts.googleapis.com/css2?family=Syne:wght@400;600;700;800&family=DM+Sans:ital,wght@0,300;0,400;0,500;1,300&display=swap" rel="stylesheet"/>
  <style>
    :root {
      --bg: #0a0a0f;
      --surface: #111118;
      --card: #16161f;
      --border: #2a2a3a;
      --accent: #00e5a0;
      --accent2: #7c6aff;
      --accent3: #ff6b6b;
      --text: #e8e8f0;
      --muted: #7070a0;
      --heading-font: 'Syne', sans-serif;
      --body-font: 'DM Sans', sans-serif;
    }

    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    html { scroll-behavior: smooth; }

    body {
      background: var(--bg);
      color: var(--text);
      font-family: var(--body-font);
      font-size: 16px;
      line-height: 1.7;
      overflow-x: hidden;
    }

    /* ---- NOISE TEXTURE OVERLAY ---- */
    body::before {
      content: '';
      position: fixed; inset: 0;
      background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 512 512' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)' opacity='0.04'/%3E%3C/svg%3E");
      pointer-events: none;
      z-index: 9999;
      opacity: 0.4;
    }

    /* ---- NAV ---- */
    nav {
      position: fixed; top: 0; left: 0; right: 0;
      display: flex; align-items: center; justify-content: space-between;
      padding: 1.2rem 5%;
      background: rgba(10,10,15,0.85);
      backdrop-filter: blur(20px);
      border-bottom: 1px solid var(--border);
      z-index: 1000;
    }
    .nav-logo {
      font-family: var(--heading-font);
      font-size: 1.4rem;
      font-weight: 800;
      color: var(--accent);
      letter-spacing: -0.5px;
    }
    .nav-logo span { color: var(--text); }
    .nav-links { display: flex; gap: 2rem; list-style: none; }
    .nav-links a {
      color: var(--muted);
      text-decoration: none;
      font-size: 0.9rem;
      font-weight: 500;
      letter-spacing: 0.3px;
      transition: color 0.2s;
    }
    .nav-links a:hover { color: var(--accent); }
    .nav-cta {
      background: var(--accent);
      color: #000;
      border: none;
      padding: 0.55rem 1.3rem;
      border-radius: 6px;
      font-family: var(--heading-font);
      font-weight: 700;
      font-size: 0.85rem;
      cursor: pointer;
      letter-spacing: 0.5px;
      transition: transform 0.15s, box-shadow 0.15s;
    }
    .nav-cta:hover { transform: translateY(-1px); box-shadow: 0 6px 20px rgba(0,229,160,0.35); }

    /* ---- HERO ---- */
    #hero {
      min-height: 100vh;
      display: flex; align-items: center;
      padding: 6rem 5% 4rem;
      position: relative;
      overflow: hidden;
    }
    .hero-glow {
      position: absolute;
      width: 600px; height: 600px;
      border-radius: 50%;
      background: radial-gradient(circle, rgba(0,229,160,0.12) 0%, transparent 70%);
      top: -100px; right: -100px;
      animation: pulse 6s ease-in-out infinite;
    }
    .hero-glow2 {
      position: absolute;
      width: 400px; height: 400px;
      border-radius: 50%;
      background: radial-gradient(circle, rgba(124,106,255,0.1) 0%, transparent 70%);
      bottom: 0; left: 10%;
      animation: pulse 8s ease-in-out infinite reverse;
    }
    @keyframes pulse {
      0%, 100% { transform: scale(1); opacity: 1; }
      50% { transform: scale(1.15); opacity: 0.7; }
    }
    .hero-content { max-width: 700px; position: relative; z-index: 1; }
    .hero-badge {
      display: inline-flex; align-items: center; gap: 0.5rem;
      background: rgba(0,229,160,0.1);
      border: 1px solid rgba(0,229,160,0.3);
      padding: 0.4rem 1rem;
      border-radius: 100px;
      font-size: 0.8rem;
      color: var(--accent);
      font-weight: 500;
      margin-bottom: 1.5rem;
      animation: fadeUp 0.6s ease forwards;
    }
    .dot { width: 7px; height: 7px; background: var(--accent); border-radius: 50%; animation: blink 1.5s infinite; }
    @keyframes blink { 0%, 100% { opacity: 1; } 50% { opacity: 0.2; } }

    .hero-title {
      font-family: var(--heading-font);
      font-size: clamp(2.8rem, 6vw, 5rem);
      font-weight: 800;
      line-height: 1.05;
      letter-spacing: -2px;
      margin-bottom: 1.2rem;
      animation: fadeUp 0.7s 0.1s ease both;
    }
    .hero-title .line2 { color: var(--accent); }
    .hero-title .line3 { 
      background: linear-gradient(135deg, var(--accent2), var(--accent3));
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }
    .hero-sub {
      color: var(--muted);
      font-size: 1.1rem;
      max-width: 540px;
      margin-bottom: 2.5rem;
      animation: fadeUp 0.7s 0.2s ease both;
    }
    .hero-buttons {
      display: flex; gap: 1rem; flex-wrap: wrap;
      animation: fadeUp 0.7s 0.3s ease both;
    }
    .btn-primary {
      background: var(--accent);
      color: #000;
      padding: 0.85rem 2rem;
      border-radius: 8px;
      font-family: var(--heading-font);
      font-weight: 700;
      font-size: 0.95rem;
      text-decoration: none;
      letter-spacing: 0.3px;
      transition: transform 0.15s, box-shadow 0.15s;
      display: inline-block;
    }
    .btn-primary:hover { transform: translateY(-2px); box-shadow: 0 10px 30px rgba(0,229,160,0.4); }
    .btn-secondary {
      background: transparent;
      color: var(--text);
      padding: 0.85rem 2rem;
      border-radius: 8px;
      font-family: var(--heading-font);
      font-weight: 700;
      font-size: 0.95rem;
      text-decoration: none;
      border: 1px solid var(--border);
      transition: border-color 0.2s, color 0.2s;
      display: inline-block;
    }
    .btn-secondary:hover { border-color: var(--accent); color: var(--accent); }

    .hero-stats {
      display: flex; gap: 3rem; margin-top: 3.5rem;
      animation: fadeUp 0.7s 0.4s ease both;
      padding-top: 2.5rem;
      border-top: 1px solid var(--border);
    }
    .stat-num {
      font-family: var(--heading-font);
      font-size: 2rem;
      font-weight: 800;
      color: var(--accent);
    }
    .stat-label { font-size: 0.8rem; color: var(--muted); margin-top: 0.1rem; }

    @keyframes fadeUp {
      from { opacity: 0; transform: translateY(24px); }
      to { opacity: 1; transform: translateY(0); }
    }

    /* ---- SECTIONS ---- */
    section { padding: 5rem 5%; }
    .section-label {
      font-size: 0.75rem;
      font-weight: 700;
      letter-spacing: 3px;
      text-transform: uppercase;
      color: var(--accent);
      margin-bottom: 0.7rem;
    }
    .section-title {
      font-family: var(--heading-font);
      font-size: clamp(1.8rem, 3.5vw, 2.8rem);
      font-weight: 800;
      letter-spacing: -1px;
      line-height: 1.15;
      margin-bottom: 1rem;
    }
    .section-sub { color: var(--muted); max-width: 520px; font-size: 1rem; }

    /* ---- SERVICES ---- */
    #services { background: var(--surface); }
    .services-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 1.5rem;
      margin-top: 3rem;
    }
    .service-card {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: 16px;
      padding: 2rem;
      transition: transform 0.2s, border-color 0.2s, box-shadow 0.2s;
      position: relative;
      overflow: hidden;
    }
    .service-card::before {
      content: '';
      position: absolute; top: 0; left: 0; right: 0;
      height: 2px;
      background: linear-gradient(90deg, var(--accent), var(--accent2));
      opacity: 0;
      transition: opacity 0.2s;
    }
    .service-card:hover { transform: translateY(-4px); border-color: rgba(0,229,160,0.3); box-shadow: 0 20px 40px rgba(0,0,0,0.4); }
    .service-card:hover::before { opacity: 1; }
    .service-icon {
      width: 50px; height: 50px;
      background: rgba(0,229,160,0.1);
      border-radius: 12px;
      display: flex; align-items: center; justify-content: center;
      font-size: 1.5rem;
      margin-bottom: 1.2rem;
    }
    .service-title {
      font-family: var(--heading-font);
      font-size: 1.15rem;
      font-weight: 700;
      margin-bottom: 0.6rem;
    }
    .service-desc { color: var(--muted); font-size: 0.9rem; line-height: 1.65; }
    .service-tags { display: flex; flex-wrap: wrap; gap: 0.4rem; margin-top: 1.2rem; }
    .tag {
      font-size: 0.72rem;
      padding: 0.25rem 0.7rem;
      border-radius: 100px;
      background: rgba(124,106,255,0.1);
      color: var(--accent2);
      border: 1px solid rgba(124,106,255,0.2);
      font-weight: 500;
    }

    /* ---- PORTFOLIO ---- */
    #portfolio { }
    .portfolio-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
      gap: 1.5rem;
      margin-top: 3rem;
    }
    .portfolio-card {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: 16px;
      overflow: hidden;
      transition: transform 0.2s, box-shadow 0.2s;
    }
    .portfolio-card:hover { transform: translateY(-4px); box-shadow: 0 24px 50px rgba(0,0,0,0.5); }
    .portfolio-thumb {
      height: 180px;
      display: flex; align-items: center; justify-content: center;
      font-size: 3rem;
      position: relative;
      overflow: hidden;
    }
    .thumb-1 { background: linear-gradient(135deg, #0a2a1a, #0d3d25); }
    .thumb-2 { background: linear-gradient(135deg, #1a0a2a, #2d0d3d); }
    .thumb-3 { background: linear-gradient(135deg, #2a1a0a, #3d2d0d); }
    .portfolio-info { padding: 1.5rem; }
    .portfolio-cat {
      font-size: 0.72rem;
      color: var(--accent);
      font-weight: 600;
      letter-spacing: 1.5px;
      text-transform: uppercase;
      margin-bottom: 0.4rem;
    }
    .portfolio-name {
      font-family: var(--heading-font);
      font-size: 1.1rem;
      font-weight: 700;
      margin-bottom: 0.5rem;
    }
    .portfolio-desc { color: var(--muted); font-size: 0.88rem; }
    .portfolio-metrics {
      display: flex; gap: 1.5rem; margin-top: 1rem;
      padding-top: 1rem; border-top: 1px solid var(--border);
    }
    .metric-val {
      font-family: var(--heading-font);
      font-size: 1.1rem;
      font-weight: 700;
      color: var(--accent);
    }
    .metric-label { font-size: 0.72rem; color: var(--muted); }

    /* ---- PRICING ---- */
    #pricing { background: var(--surface); }
    .pricing-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 1.5rem;
      margin-top: 3rem;
      align-items: start;
    }
    .pricing-card {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: 20px;
      padding: 2.2rem;
      transition: transform 0.2s;
      position: relative;
    }
    .pricing-card.featured {
      border-color: var(--accent);
      background: linear-gradient(160deg, rgba(0,229,160,0.05), var(--card));
      transform: scale(1.03);
    }
    .featured-badge {
      position: absolute;
      top: -14px; left: 50%; transform: translateX(-50%);
      background: var(--accent);
      color: #000;
      font-family: var(--heading-font);
      font-size: 0.7rem;
      font-weight: 800;
      padding: 0.3rem 1rem;
      border-radius: 100px;
      letter-spacing: 1px;
      text-transform: uppercase;
    }
    .plan-name {
      font-family: var(--heading-font);
      font-size: 1rem;
      font-weight: 700;
      color: var(--muted);
      margin-bottom: 0.8rem;
      letter-spacing: 1px;
      text-transform: uppercase;
    }
    .plan-price {
      font-family: var(--heading-font);
      font-size: 2.5rem;
      font-weight: 800;
      color: var(--text);
      line-height: 1;
      margin-bottom: 0.3rem;
    }
    .plan-price span { font-size: 1rem; color: var(--muted); font-weight: 400; }
    .plan-desc { color: var(--muted); font-size: 0.88rem; margin-bottom: 1.8rem; }
    .plan-features { list-style: none; margin-bottom: 2rem; }
    .plan-features li {
      padding: 0.55rem 0;
      font-size: 0.9rem;
      border-bottom: 1px solid rgba(255,255,255,0.04);
      display: flex; align-items: center; gap: 0.7rem;
      color: var(--text);
    }
    .plan-features li::before { content: '✓'; color: var(--accent); font-weight: 700; font-size: 0.8rem; }
    .plan-features li.no::before { content: '×'; color: var(--muted); }
    .plan-features li.no { color: var(--muted); }
    .btn-plan {
      width: 100%;
      padding: 0.9rem;
      border-radius: 10px;
      font-family: var(--heading-font);
      font-weight: 700;
      font-size: 0.9rem;
      cursor: pointer;
      letter-spacing: 0.3px;
      transition: all 0.2s;
    }
    .btn-plan-outline {
      background: transparent;
      color: var(--text);
      border: 1px solid var(--border);
    }
    .btn-plan-outline:hover { border-color: var(--accent); color: var(--accent); }
    .btn-plan-solid {
      background: var(--accent);
      color: #000;
      border: none;
    }
    .btn-plan-solid:hover { box-shadow: 0 8px 25px rgba(0,229,160,0.4); transform: translateY(-1px); }

    /* ---- BLOG ---- */
    #blog { }
    .blog-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 1.5rem;
      margin-top: 3rem;
    }
    .blog-card {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: 16px;
      overflow: hidden;
      transition: transform 0.2s, box-shadow 0.2s;
      text-decoration: none;
      color: inherit;
      display: block;
    }
    .blog-card:hover { transform: translateY(-4px); box-shadow: 0 20px 40px rgba(0,0,0,0.4); }
    .blog-header {
      padding: 1.5rem;
      border-bottom: 1px solid var(--border);
      display: flex; align-items: center; gap: 0.8rem;
    }
    .blog-num {
      font-family: var(--heading-font);
      font-size: 2rem;
      font-weight: 800;
      color: var(--border);
      line-height: 1;
    }
    .blog-cat {
      font-size: 0.72rem;
      color: var(--accent2);
      font-weight: 600;
      letter-spacing: 1.5px;
      text-transform: uppercase;
    }
    .blog-body { padding: 1.5rem; }
    .blog-title {
      font-family: var(--heading-font);
      font-size: 1.05rem;
      font-weight: 700;
      line-height: 1.4;
      margin-bottom: 0.7rem;
    }
    .blog-snippet { color: var(--muted); font-size: 0.88rem; line-height: 1.6; }
    .blog-footer {
      padding: 1rem 1.5rem;
      border-top: 1px solid var(--border);
      display: flex; justify-content: space-between; align-items: center;
    }
    .blog-date { font-size: 0.78rem; color: var(--muted); }
    .blog-read {
      font-size: 0.78rem;
      color: var(--accent);
      font-weight: 600;
    }

    /* ---- CONTACT ---- */
    #contact { background: var(--surface); }
    .contact-grid {
      display: grid;
      grid-template-columns: 1fr 1.6fr;
      gap: 4rem;
      margin-top: 3rem;
      align-items: start;
    }
    .contact-info h3 {
      font-family: var(--heading-font);
      font-size: 1.4rem;
      font-weight: 700;
      margin-bottom: 1rem;
    }
    .contact-info p { color: var(--muted); font-size: 0.95rem; line-height: 1.7; margin-bottom: 2rem; }
    .contact-item {
      display: flex; align-items: center; gap: 1rem;
      margin-bottom: 1.2rem;
    }
    .contact-icon {
      width: 42px; height: 42px;
      background: rgba(0,229,160,0.1);
      border-radius: 10px;
      display: flex; align-items: center; justify-content: center;
      font-size: 1.1rem;
      flex-shrink: 0;
    }
    .contact-item-label { font-size: 0.75rem; color: var(--muted); }
    .contact-item-val { font-size: 0.95rem; font-weight: 500; }

    /* FORM */
    .contact-form { display: flex; flex-direction: column; gap: 1.2rem; }
    .form-row { display: grid; grid-template-columns: 1fr 1fr; gap: 1rem; }
    .form-group { display: flex; flex-direction: column; gap: 0.4rem; }
    .form-group label { font-size: 0.82rem; color: var(--muted); font-weight: 500; }
    .form-group input,
    .form-group select,
    .form-group textarea {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: 10px;
      padding: 0.85rem 1rem;
      color: var(--text);
      font-family: var(--body-font);
      font-size: 0.92rem;
      transition: border-color 0.2s, box-shadow 0.2s;
      outline: none;
    }
    .form-group input:focus,
    .form-group select:focus,
    .form-group textarea:focus {
      border-color: var(--accent);
      box-shadow: 0 0 0 3px rgba(0,229,160,0.1);
    }
    .form-group textarea { resize: vertical; min-height: 130px; }
    .form-group select option { background: var(--card); }
    .btn-submit {
      background: var(--accent);
      color: #000;
      border: none;
      padding: 1rem;
      border-radius: 10px;
      font-family: var(--heading-font);
      font-weight: 700;
      font-size: 0.95rem;
      cursor: pointer;
      letter-spacing: 0.3px;
      transition: transform 0.15s, box-shadow 0.15s;
      margin-top: 0.5rem;
    }
    .btn-submit:hover { transform: translateY(-2px); box-shadow: 0 10px 30px rgba(0,229,160,0.4); }

    /* ---- FOOTER ---- */
    footer {
      background: #070709;
      padding: 3rem 5% 2rem;
      border-top: 1px solid var(--border);
    }
    .footer-top {
      display: flex; justify-content: space-between; align-items: center;
      margin-bottom: 2rem;
      padding-bottom: 2rem;
      border-bottom: 1px solid var(--border);
    }
    .footer-logo {
      font-family: var(--heading-font);
      font-size: 1.3rem;
      font-weight: 800;
      color: var(--accent);
    }
    .footer-links { display: flex; gap: 2rem; }
    .footer-links a { color: var(--muted); text-decoration: none; font-size: 0.88rem; transition: color 0.2s; }
    .footer-links a:hover { color: var(--accent); }
    .footer-bottom {
      display: flex; justify-content: space-between; align-items: center;
    }
    .footer-copy { color: var(--muted); font-size: 0.82rem; }
    .footer-seo-note {
      font-size: 0.78rem;
      color: rgba(0,229,160,0.5);
      font-style: italic;
    }

    /* ---- SCROLL REVEAL ---- */
    .reveal {
      opacity: 0;
      transform: translateY(30px);
      transition: opacity 0.65s ease, transform 0.65s ease;
    }
    .reveal.visible {
      opacity: 1;
      transform: translateY(0);
    }

    /* ---- RESPONSIVE ---- */
    @media (max-width: 768px) {
      .nav-links { display: none; }
      .hero-stats { gap: 1.5rem; flex-wrap: wrap; }
      .contact-grid { grid-template-columns: 1fr; gap: 2.5rem; }
      .form-row { grid-template-columns: 1fr; }
      .footer-top { flex-direction: column; gap: 1.5rem; text-align: center; }
      .footer-bottom { flex-direction: column; gap: 0.5rem; text-align: center; }
      .pricing-card.featured { transform: scale(1); }
    }
  </style>
</head>
<body>

  <!-- NAV -->
  <nav>
    <div class="nav-logo">SEO with <span>Tehzeeb</span></div>
    <ul class="nav-links">
      <li><a href="#services">Services</a></li>
      <li><a href="#portfolio">Portfolio</a></li>
      <li><a href="#pricing">Pricing</a></li>
      <li><a href="#blog">Blog</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
    <button class="nav-cta" onclick="document.getElementById('contact').scrollIntoView({behavior:'smooth'})">Hire Me</button>
  </nav>

  <!-- HERO -->
  <section id="hero">
    <div class="hero-glow"></div>
    <div class="hero-glow2"></div>
    <div class="hero-content">
      <div class="hero-badge">
        <span class="dot"></span>
        Available for New Projects
      </div>
      <h1 class="hero-title">
        SEO That<br>
        <span class="line2">Actually Ranks.</span><br>
        <span class="line3">Results That Last.</span>
      </h1>
      <p class="hero-sub">
        I help businesses rank higher on Google, grow organic traffic, and convert visitors into customers — using data-driven SEO, digital marketing, and AI-powered strategies.
      </p>
      <div class="hero-buttons">
        <a href="#portfolio" class="btn-primary">View My Work</a>
        <a href="#contact" class="btn-secondary">Let's Talk →</a>
      </div>
      <div class="hero-stats">
        <div>
          <div class="stat-num">50+</div>
          <div class="stat-label">Keywords Ranked</div>
        </div>
        <div>
          <div class="stat-num">3x</div>
          <div class="stat-label">Avg Traffic Growth</div>
        </div>
        <div>
          <div class="stat-num">100%</div>
          <div class="stat-label">White-Hat SEO</div>
        </div>
      </div>
    </div>
  </section>

  <!-- SERVICES -->
  <section id="services">
    <div class="reveal">
      <div class="section-label">What I Do</div>
      <h2 class="section-title">Services Designed<br>to Grow Your Business</h2>
      <p class="section-sub">From technical SEO audits to AI-powered content — complete digital marketing solutions for modern businesses.</p>
    </div>
    <div class="services-grid">
      <div class="service-card reveal">
        <div class="service-icon">🔍</div>
        <div class="service-title">Search Engine Optimization</div>
        <p class="service-desc">Full-funnel SEO strategy — on-page, off-page, technical audits, keyword research, and competitor analysis to dominate search results.</p>
        <div class="service-tags">
          <span class="tag">On-Page SEO</span>
          <span class="tag">Technical SEO</span>
          <span class="tag">Link Building</span>
        </div>
      </div>
      <div class="service-card reveal">
        <div class="service-icon">📈</div>
        <div class="service-title">Digital Marketing Strategy</div>
        <p class="service-desc">End-to-end digital marketing campaigns — social media, email, content, and paid ads working together to maximize your ROI.</p>
        <div class="service-tags">
          <span class="tag">Social Media</span>
          <span class="tag">Content Strategy</span>
          <span class="tag">Email Marketing</span>
        </div>
      </div>
      <div class="service-card reveal">
        <div class="service-icon">🤖</div>
        <div class="service-title">AI-Powered Content & Marketing</div>
        <p class="service-desc">Leverage generative AI to scale content production, automate workflows, and create hyper-personalized marketing at scale.</p>
        <div class="service-tags">
          <span class="tag">AI Content</span>
          <span class="tag">ChatGPT</span>
          <span class="tag">Automation</span>
        </div>
      </div>
      <div class="service-card reveal">
        <div class="service-icon">🔧</div>
        <div class="service-title">Technical SEO Audit</div>
        <p class="service-desc">Deep-dive site audits covering Core Web Vitals, crawlability, schema markup, site speed, and mobile optimization.</p>
        <div class="service-tags">
          <span class="tag">Core Web Vitals</span>
          <span class="tag">Schema</span>
          <span class="tag">Site Speed</span>
        </div>
      </div>
      <div class="service-card reveal">
        <div class="service-icon">📝</div>
        <div class="service-title">SEO Content Writing</div>
        <p class="service-desc">Keyword-optimized, human-first content that ranks on Google AND converts readers into customers. Blog posts, landing pages, product descriptions.</p>
        <div class="service-tags">
          <span class="tag">Blog Posts</span>
          <span class="tag">Landing Pages</span>
          <span class="tag">Copywriting</span>
        </div>
      </div>
      <div class="service-card reveal">
        <div class="service-icon">📊</div>
        <div class="service-title">Analytics & Reporting</div>
        <p class="service-desc">Custom Google Analytics 4, Search Console dashboards, and monthly reports that turn data into clear, actionable insights.</p>
        <div class="service-tags">
          <span class="tag">GA4</span>
          <span class="tag">Search Console</span>
          <span class="tag">Monthly Reports</span>
        </div>
      </div>
    </div>
  </section>

  <!-- PORTFOLIO -->
  <section id="portfolio">
    <div class="reveal">
      <div class="section-label">My Work</div>
      <h2 class="section-title">Projects & Results</h2>
      <p class="section-sub">Real-world SEO projects with measurable outcomes — ranking improvements, traffic growth, and business results.</p>
    </div>
    <div class="portfolio-grid">
      <div class="portfolio-card reveal">
        <div class="portfolio-thumb thumb-1">🛒</div>
        <div class="portfolio-info">
          <div class="portfolio-cat">E-commerce SEO</div>
          <div class="portfolio-name">Online Store — Organic Growth</div>
          <p class="portfolio-desc">Full SEO overhaul for an e-commerce store. Keyword research, product page optimization, blog content strategy, and link building.</p>
          <div class="portfolio-metrics">
            <div>
              <div class="metric-val">+187%</div>
              <div class="metric-label">Organic Traffic</div>
            </div>
            <div>
              <div class="metric-val">Page 1</div>
              <div class="metric-label">32 Keywords</div>
            </div>
            <div>
              <div class="metric-val">4 Months</div>
              <div class="metric-label">Timeline</div>
            </div>
          </div>
        </div>
      </div>
      <div class="portfolio-card reveal">
        <div class="portfolio-thumb thumb-2">💼</div>
        <div class="portfolio-info">
          <div class="portfolio-cat">Local SEO</div>
          <div class="portfolio-name">Local Business — Google Maps Rank</div>
          <p class="portfolio-desc">Local SEO campaign for a service business. Google My Business optimization, local citations, and review strategy.</p>
          <div class="portfolio-metrics">
            <div>
              <div class="metric-val">#1</div>
              <div class="metric-label">Google Maps</div>
            </div>
            <div>
              <div class="metric-val">+240%</div>
              <div class="metric-label">Calls from Search</div>
            </div>
            <div>
              <div class="metric-val">3 Months</div>
              <div class="metric-label">Timeline</div>
            </div>
          </div>
        </div>
      </div>
      <div class="portfolio-card reveal">
        <div class="portfolio-thumb thumb-3">🤖</div>
        <div class="portfolio-info">
          <div class="portfolio-cat">AI Content Strategy</div>
          <div class="portfolio-name">Blog — AI-Assisted Content at Scale</div>
          <p class="portfolio-desc">Used generative AI tools to build a content pipeline of 40+ SEO articles in 6 weeks, all optimized and published.</p>
          <div class="portfolio-metrics">
            <div>
              <div class="metric-val">40+</div>
              <div class="metric-label">Articles Published</div>
            </div>
            <div>
              <div class="metric-val">+320%</div>
              <div class="metric-label">Blog Traffic</div>
            </div>
            <div>
              <div class="metric-val">6 Weeks</div>
              <div class="metric-label">Timeline</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- PRICING -->
  <section id="pricing">
    <div class="reveal">
      <div class="section-label">Pricing Plans</div>
      <h2 class="section-title">Simple, Transparent<br>Pricing</h2>
      <p class="section-sub">No hidden fees. Pick the plan that fits your goals. All plans include monthly reports and direct communication.</p>
    </div>
    <div class="pricing-grid">
      <!-- Starter -->
      <div class="pricing-card reveal">
        <div class="plan-name">Starter</div>
        <div class="plan-price">$99 <span>/ month</span></div>
        <p class="plan-desc">Perfect for small businesses just getting started with SEO.</p>
        <ul class="plan-features">
          <li>SEO Audit (10 pages)</li>
          <li>5 Target Keywords</li>
          <li>On-Page Optimization</li>
          <li>Monthly Report</li>
          <li>Google Search Console Setup</li>
          <li class="no">Link Building</li>
          <li class="no">Content Writing</li>
        </ul>
        <button class="btn-plan btn-plan-outline" onclick="document.getElementById('contact').scrollIntoView({behavior:'smooth'})">Get Started</button>
      </div>
      <!-- Growth (Featured) -->
      <div class="pricing-card featured reveal">
        <div class="featured-badge">Most Popular</div>
        <div class="plan-name">Growth</div>
        <div class="plan-price">$249 <span>/ month</span></div>
        <p class="plan-desc">Best for growing businesses that want real, measurable results.</p>
        <ul class="plan-features">
          <li>Full SEO Audit</li>
          <li>15 Target Keywords</li>
          <li>On-Page + Technical SEO</li>
          <li>4 Blog Articles / Month</li>
          <li>Link Building (5 links)</li>
          <li>Google Analytics 4 Setup</li>
          <li>Bi-weekly Reports</li>
        </ul>
        <button class="btn-plan btn-plan-solid" onclick="document.getElementById('contact').scrollIntoView({behavior:'smooth'})">Hire Me Now</button>
      </div>
      <!-- Pro -->
      <div class="pricing-card reveal">
        <div class="plan-name">Pro / Agency</div>
        <div class="plan-price">$499 <span>/ month</span></div>
        <p class="plan-desc">Full-service digital marketing for ambitious brands and agencies.</p>
        <ul class="plan-features">
          <li>Everything in Growth</li>
          <li>30+ Target Keywords</li>
          <li>AI Content Strategy</li>
          <li>8 Blog Articles / Month</li>
          <li>Link Building (15 links)</li>
          <li>Social Media Strategy</li>
          <li>Weekly Reports + Calls</li>
        </ul>
        <button class="btn-plan btn-plan-outline" onclick="document.getElementById('contact').scrollIntoView({behavior:'smooth'})">Contact Me</button>
      </div>
    </div>
  </section>

  <!-- BLOG -->
  <section id="blog">
    <div class="reveal">
      <div class="section-label">Knowledge Hub</div>
      <h2 class="section-title">SEO & Marketing Tips</h2>
      <p class="section-sub">Practical guides, tutorials, and insights to help you grow your online presence — updated regularly.</p>
    </div>
    <div class="blog-grid">
      <a href="#blog" class="blog-card reveal">
        <div class="blog-header">
          <div class="blog-num">01</div>
          <div><div class="blog-cat">SEO Guide</div></div>
        </div>
        <div class="blog-body">
          <div class="blog-title">How to Do Keyword Research in 2024: A Beginner's Guide</div>
          <p class="blog-snippet">Learn how to find profitable keywords with zero budget using Google Search Console, Ubersuggest, and free tools that actually work.</p>
        </div>
        <div class="blog-footer">
          <span class="blog-date">Jan 2025</span>
          <span class="blog-read">Read More →</span>
        </div>
      </a>
      <a href="#blog" class="blog-card reveal">
        <div class="blog-header">
          <div class="blog-num">02</div>
          <div><div class="blog-cat">AI Marketing</div></div>
        </div>
        <div class="blog-body">
          <div class="blog-title">Using ChatGPT for SEO: 10 Prompts That Save Hours of Work</div>
          <p class="blog-snippet">Discover how to use generative AI to write meta descriptions, generate title ideas, create content briefs, and automate your SEO workflow.</p>
        </div>
        <div class="blog-footer">
          <span class="blog-date">Feb 2025</span>
          <span class="blog-read">Read More →</span>
        </div>
      </a>
      <a href="#blog" class="blog-card reveal">
        <div class="blog-header">
          <div class="blog-num">03</div>
          <div><div class="blog-cat">Technical SEO</div></div>
        </div>
        <div class="blog-body">
          <div class="blog-title">Core Web Vitals 2025: What Actually Matters for Rankings</div>
          <p class="blog-snippet">A plain-English breakdown of LCP, CLS, and INP — what they are, how to measure them, and quick wins to improve your scores today.</p>
        </div>
        <div class="blog-footer">
          <span class="blog-date">Mar 2025</span>
          <span class="blog-read">Read More →</span>
        </div>
      </a>
    </div>
  </section>

  <!-- CONTACT -->
  <section id="contact">
    <div class="reveal">
      <div class="section-label">Get In Touch</div>
      <h2 class="section-title">Let's Work Together</h2>
      <p class="section-sub">Have a project in mind? Send me a message and I'll get back to you within 24 hours.</p>
    </div>
    <div class="contact-grid">
      <div class="reveal">
        <h3>Hire Me for Your Next Project</h3>
        <p>Whether you need a one-time SEO audit or a long-term growth partner, I'm here to help your business rank higher and grow faster.</p>
        <div class="contact-item">
          <div class="contact-icon">📧</div>
          <div>
            <div class="contact-item-label">Email</div>
            <div class="contact-item-val">SEOWithTehzeeb@gmail.com</div>
          </div>
        </div>
        <div class="contact-item">
          <div class="contact-icon">💬</div>
          <div>
            <div class="contact-item-label">WhatsApp</div>
            <div class="contact-item-val">0342-521-1509</div>
          </div>
        </div>
        <div class="contact-item">
          <div class="contact-icon">🌐</div>
          <div>
            <div class="contact-item-label">Freelance Platforms</div>
            <div class="contact-item-val">Upwork · Fiverr · LinkedIn</div>
          </div>
        </div>
        <div class="contact-item">
          <div class="contact-icon">⏱️</div>
          <div>
            <div class="contact-item-label">Response Time</div>
            <div class="contact-item-val">Within 24 hours</div>
          </div>
        </div>
      </div>
      <div class="reveal">
        <form class="contact-form" onsubmit="handleSubmit(event)">
          <div class="form-row">
            <div class="form-group">
              <label for="name">Your Name</label>
              <input type="text" id="name" placeholder="Ahmed Khan" required />
            </div>
            <div class="form-group">
              <label for="email">Email Address</label>
              <input type="email" id="email" placeholder="ahmed@example.com" required />
            </div>
          </div>
          <div class="form-group">
            <label for="service">Service Needed</label>
            <select id="service">
              <option value="">Select a service...</option>
              <option>SEO Audit</option>
              <option>On-Page SEO</option>
              <option>Full SEO Campaign</option>
              <option>AI Content Strategy</option>
              <option>Digital Marketing</option>
              <option>Other</option>
            </select>
          </div>
          <div class="form-group">
            <label for="budget">Budget Range</label>
            <select id="budget">
              <option value="">Select budget...</option>
              <option>Under $100</option>
              <option>$100 – $300</option>
              <option>$300 – $500</option>
              <option>$500+</option>
            </select>
          </div>
          <div class="form-group">
            <label for="message">Tell Me About Your Project</label>
            <textarea id="message" placeholder="I need help ranking my website for [keywords]..."></textarea>
          </div>
          <button type="submit" class="btn-submit">Send Message 🚀</button>
        </form>
      </div>
    </div>
  </section>

  <!-- FOOTER -->
  <footer>
    <div class="footer-top">
      <div class="footer-logo">SEO with Tehzeeb</div>
      <div class="footer-links">
        <a href="#services">Services</a>
        <a href="#portfolio">Portfolio</a>
        <a href="#pricing">Pricing</a>
        <a href="#blog">Blog</a>
        <a href="#contact">Contact</a>
      </div>
    </div>
    <div class="footer-bottom">
      <div class="footer-copy">© 2025 SEO with Tehzeeb. SEO & Digital Marketing Freelancer.</div>
      <div class="footer-seo-note">Built with SEO best practices · Schema ready · Fast loading</div>
    </div>
  </footer>

  <script>
    // Scroll Reveal
    const reveals = document.querySelectorAll('.reveal');
    const observer = new IntersectionObserver(entries => {
      entries.forEach(e => { if (e.isIntersecting) e.target.classList.add('visible'); });
    }, { threshold: 0.1 });
    reveals.forEach(r => observer.observe(r));

    // Contact Form
    function handleSubmit(e) {
      e.preventDefault();
      const btn = e.target.querySelector('.btn-submit');
      btn.textContent = '✅ Message Sent!';
      btn.style.background = '#16a34a';
      setTimeout(() => {
        btn.textContent = 'Send Message 🚀';
        btn.style.background = '';
        e.target.reset();
      }, 3000);
    }
  </script>
</body>
</html>
