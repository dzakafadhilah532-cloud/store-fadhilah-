<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Dzaka Irfan Fadhilah · Profil Profesional</title>
  <meta name="description" content="Portfolio profesional Dzaka Irfan Fadhilah – UI/UX Designer & Pengembang Web." />
  <meta property="og:title" content="Dzaka Irfan Fadhilah · Profil Profesional" />
  <meta property="og:description" content="Portfolio profesional dengan desain modern dan elegan." />
  <meta property="og:image" content="https://via.placeholder.com/1200x630.png?text=Dzaka+Irfan+Fadhilah" />
  <meta property="og:type" content="website" />
  <link rel="icon" href="data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'><text y='.9em' font-size='90'>👤</text></svg>" />
  
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Inter:opsz@14..32&family=Plus+Jakarta+Sans:wght@400;500;600;700&display=swap" rel="stylesheet" />
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" />
  <style>
    /* ----- RESET & GLOBAL ----- */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Inter', 'Plus Jakarta Sans', sans-serif;
      background: #fcfcfc;
      color: #1e1e1e;
      line-height: 1.6;
      scroll-behavior: smooth;
      transition: background 0.3s, color 0.3s;
    }
    body.dark {
      background: #141414;
      color: #eaeaea;
    }
    a { text-decoration: none; color: inherit; }
    img { max-width: 100%; display: block; }
    .container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 1.5rem;
    }

    /* ----- NAVBAR (sticky + hamburger) ----- */
    .navbar {
      position: sticky;
      top: 0;
      z-index: 999;
      background: rgba(252, 252, 252, 0.85);
      backdrop-filter: blur(10px);
      border-bottom: 1px solid rgba(0,0,0,0.04);
      padding: 0.75rem 0;
      transition: background 0.2s;
    }
    body.dark .navbar {
      background: rgba(20, 20, 20, 0.9);
      border-bottom: 1px solid rgba(255,255,255,0.05);
    }
    .navbar .container {
      display: flex;
      align-items: center;
      justify-content: space-between;
    }
    .logo {
      font-weight: 700;
      font-size: 1.4rem;
      letter-spacing: -0.5px;
    }
    .logo span { color: #0b3b5c; }
    body.dark .logo span { color: #6ab0e6; }

    .nav-menu {
      display: flex;
      align-items: center;
      gap: 1.8rem;
      list-style: none;
    }
    .nav-menu a {
      font-size: 0.95rem;
      font-weight: 500;
      color: #2c2c2c;
      transition: 0.15s;
      position: relative;
    }
    body.dark .nav-menu a { color: #cfcfcf; }
    .nav-menu a::after {
      content: '';
      position: absolute;
      bottom: -4px;
      left: 0;
      width: 0;
      height: 2px;
      background: #0b3b5c;
      transition: 0.2s;
    }
    body.dark .nav-menu a::after { background: #6ab0e6; }
    .nav-menu a:hover::after,
    .nav-menu a.active::after { width: 100%; }

    .hamburger {
      display: none;
      font-size: 1.7rem;
      background: none;
      border: none;
      color: inherit;
      cursor: pointer;
    }

    .theme-toggle {
      background: none;
      border: none;
      font-size: 1.3rem;
      cursor: pointer;
      color: #2c2c2c;
      margin-left: 0.5rem;
    }
    body.dark .theme-toggle { color: #eaeaea; }

    @media (max-width: 860px) {
      .hamburger { display: block; }
      .nav-menu {
        position: absolute;
        top: 100%;
        left: 0;
        width: 100%;
        background: rgba(252, 252, 252, 0.98);
        backdrop-filter: blur(6px);
        flex-direction: column;
        padding: 1.2rem 1.5rem;
        gap: 1.2rem;
        border-top: 1px solid #eee;
        display: none;
      }
      body.dark .nav-menu {
        background: rgba(20, 20, 20, 0.98);
        border-top: 1px solid #2a2a2a;
      }
      .nav-menu.open { display: flex; }
      .theme-toggle { margin-left: auto; }
    }

    /* ----- SECTIONS ----- */
    section {
      padding: 4rem 0;
      scroll-margin-top: 80px;
    }
    .section-title {
      font-size: 2.1rem;
      font-weight: 600;
      letter-spacing: -0.02em;
      margin-bottom: 2rem;
      position: relative;
    }
    .section-title span { color: #0b3b5c; }
    body.dark .section-title span { color: #6ab0e6; }

    /* ----- HERO ----- */
    .hero {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      gap: 2.5rem;
      padding: 1rem 0 2rem;
    }
    .hero-content { flex: 1 1 300px; }
    .hero-image {
      flex: 0 0 220px;
      text-align: center;
    }
    .hero-image img {
      width: 200px;
      height: 200px;
      object-fit: cover;
      border-radius: 50%;
      box-shadow: 0 20px 40px rgba(0,0,0,0.05);
      border: 4px solid white;
      background: #eaeaea;
    }
    body.dark .hero-image img { border-color: #2a2a2a; }
    .hero h1 {
      font-size: 2.8rem;
      font-weight: 700;
      letter-spacing: -0.03em;
      line-height: 1.1;
    }
    .hero .subhead {
      font-size: 1.2rem;
      font-weight: 400;
      color: #4a4a4a;
      margin: 0.25rem 0 0.75rem;
    }
    body.dark .hero .subhead { color: #b0b0b0; }
    .hero .desc {
      max-width: 450px;
      margin: 0.5rem 0 1.5rem;
      color: #3a3a3a;
    }
    body.dark .hero .desc { color: #c0c0c0; }
    .btn-group {
      display: flex;
      flex-wrap: wrap;
      gap: 0.8rem;
    }
    .btn {
      display: inline-block;
      padding: 0.7rem 1.8rem;
      border-radius: 40px;
      font-weight: 500;
      border: 1px solid #d0d0d0;
      background: transparent;
      transition: 0.2s;
      cursor: pointer;
    }
    .btn-primary {
      background: #0b3b5c;
      border-color: #0b3b5c;
      color: white;
    }
    body.dark .btn-primary {
      background: #1f6790;
      border-color: #1f6790;
    }
    .btn-primary:hover {
      background: #0a2f4a;
      transform: translateY(-2px);
      box-shadow: 0 8px 20px rgba(11,59,92,0.15);
    }
    .btn-outline {
      border-color: #2c2c2c;
      color: #2c2c2c;
    }
    body.dark .btn-outline { border-color: #b0b0b0; color: #eaeaea; }
    .btn-outline:hover {
      background: #2c2c2c;
      color: white;
    }
    body.dark .btn-outline:hover { background: #eaeaea; color: #141414; }

    .stats {
      display: flex;
      flex-wrap: wrap;
      gap: 1.8rem;
      margin-top: 2.5rem;
    }
    .stat-item {
      background: white;
      padding: 0.8rem 1.5rem;
      border-radius: 20px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.02);
      border: 1px solid #f0f0f0;
      flex: 1 0 100px;
    }
    body.dark .stat-item {
      background: #1f1f1f;
      border-color: #2f2f2f;
    }
    .stat-item .number { font-weight: 700; font-size: 1.6rem; }
    .stat-item .label { font-size: 0.9rem; color: #5a5a5a; }
    body.dark .stat-item .label { color: #aaa; }

    /* ----- TENTANG ----- */
    .about-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 3rem;
      align-items: center;
    }
    .about-image img {
      border-radius: 24px;
      box-shadow: 0 16px 32px rgba(0,0,0,0.04);
      background: #ddd;
      aspect-ratio: 4/3;
      object-fit: cover;
      width: 100%;
    }
    body.dark .about-image img { background: #2a2a2a; }
    .about-text p { margin-bottom: 0.8rem; }
    .about-text .highlight { color: #0b3b5c; font-weight: 500; }
    body.dark .about-text .highlight { color: #6ab0e6; }
    @media (max-width: 700px) {
      .about-grid { grid-template-columns: 1fr; }
    }

    /* ----- CV ----- */
    .cv-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 2rem;
    }
    .cv-card {
      background: white;
      padding: 1.5rem 1.8rem;
      border-radius: 24px;
      border: 1px solid #efefef;
      box-shadow: 0 2px 8px rgba(0,0,0,0.01);
    }
    body.dark .cv-card {
      background: #1c1c1c;
      border-color: #2e2e2e;
    }
    .cv-card h3 {
      font-weight: 600;
      margin-bottom: 0.8rem;
      border-bottom: 2px solid #eaeaea;
      padding-bottom: 0.5rem;
    }
    body.dark .cv-card h3 { border-bottom-color: #2e2e2e; }
    .cv-timeline { margin-top: 0.5rem; }
    .cv-item { margin-bottom: 0.6rem; }
    .cv-item strong { display: block; }
    .cv-item .year { color: #0b3b5c; font-weight: 500; }
    body.dark .cv-item .year { color: #6ab0e6; }
    .download-cv {
      margin-top: 2rem;
      text-align: center;
    }

    /* ----- PORTFOLIO ----- */
    .filter-group {
      display: flex;
      flex-wrap: wrap;
      gap: 0.6rem 1.2rem;
      margin-bottom: 2rem;
    }
    .filter-btn {
      background: none;
      border: none;
      font-weight: 500;
      padding: 0.3rem 0.6rem;
      cursor: pointer;
      border-bottom: 2px solid transparent;
      transition: 0.15s;
    }
    .filter-btn.active {
      border-bottom-color: #0b3b5c;
      color: #0b3b5c;
    }
    body.dark .filter-btn.active { border-bottom-color: #6ab0e6; color: #6ab0e6; }
    .portfolio-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
      gap: 1.8rem;
    }
    .portfolio-item {
      background: white;
      border-radius: 24px;
      overflow: hidden;
      border: 1px solid #f0f0f0;
      transition: 0.2s;
    }
    body.dark .portfolio-item { background: #1c1c1c; border-color: #2e2e2e; }
    .portfolio-item:hover { transform: translateY(-6px); box-shadow: 0 12px 28px rgba(0,0,0,0.04); }
    .portfolio-item img {
      width: 100%;
      aspect-ratio: 4/3;
      object-fit: cover;
      background: #ddd;
    }
    .portfolio-info { padding: 1rem 1.2rem 1.2rem; }
    .portfolio-info h4 { font-weight: 600; }
    .portfolio-info .category { font-size: 0.8rem; color: #5a5a5a; }
    body.dark .portfolio-info .category { color: #aaa; }
    .portfolio-info .btn-small {
      margin-top: 0.5rem;
      display: inline-block;
      font-weight: 500;
      color: #0b3b5c;
      border-bottom: 1px solid transparent;
    }
    body.dark .portfolio-info .btn-small { color: #6ab0e6; }
    .portfolio-info .btn-small:hover { border-bottom-color: currentColor; }

    /* ----- FOTO & ARTIKEL ----- */
    .photo-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(160px, 1fr));
      gap: 0.8rem;
      margin-bottom: 2.5rem;
    }
    .photo-grid img {
      width: 100%;
      aspect-ratio: 1/1;
      object-fit: cover;
      border-radius: 16px;
      cursor: pointer;
      transition: 0.2s;
      background: #ddd;
    }
    .photo-grid img:hover { opacity: 0.85; transform: scale(0.98); }

    .lightbox-overlay {
      position: fixed;
      inset: 0;
      background: rgba(0,0,0,0.75);
      backdrop-filter: blur(6px);
      z-index: 1000;
      display: none;
      align-items: center;
      justify-content: center;
    }
    .lightbox-overlay.show { display: flex; }
    .lightbox-overlay img {
      max-width: 80%;
      max-height: 80%;
      border-radius: 20px;
      box-shadow: 0 20px 40px rgba(0,0,0,0.3);
    }
    .lightbox-close {
      position: absolute;
      top: 24px;
      right: 32px;
      font-size: 2.4rem;
      color: white;
      cursor: pointer;
    }

    .article-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(260px, 1fr));
      gap: 1.8rem;
      margin-top: 1rem;
    }
    .article-card {
      background: white;
      border-radius: 24px;
      padding: 1.2rem;
      border: 1px solid #efefef;
    }
    body.dark .article-card { background: #1c1c1c; border-color: #2e2e2e; }
    .article-card img {
      width: 100%;
      aspect-ratio: 16/9;
      object-fit: cover;
      border-radius: 16px;
      background: #ddd;
    }
    .article-card h4 { margin: 0.5rem 0 0.2rem; }
    .article-card .meta { font-size: 0.8rem; color: #5a5a5a; }
    body.dark .article-card .meta { color: #aaa; }

    /* ----- MEDIA SOSIAL ----- */
    .social-grid {
      display: flex;
      flex-wrap: wrap;
      gap: 1.2rem;
      justify-content: center;
    }
    .social-card {
      background: white;
      padding: 0.9rem 1.5rem;
      border-radius: 40px;
      border: 1px solid #eee;
      display: inline-flex;
      align-items: center;
      gap: 0.6rem;
      transition: 0.15s;
    }
    body.dark .social-card { background: #1c1c1c; border-color: #2e2e2e; }
    .social-card:hover { transform: translateY(-4px); box-shadow: 0 8px 16px rgba(0,0,0,0.03); }
    .social-card i { font-size: 1.5rem; width: 1.8rem; text-align: center; }

    /* ----- KONTAK ----- */
    .contact-wrap {
      display: grid;
      grid-template-columns: 1fr 1.2fr;
      gap: 2.5rem;
    }
    .contact-info p { margin: 0.5rem 0; }
    .contact-info i { width: 1.8rem; }
    .contact-form input, .contact-form textarea {
      width: 100%;
      padding: 0.8rem 1rem;
      border: 1px solid #ddd;
      border-radius: 16px;
      margin-bottom: 1rem;
      background: white;
      font-family: inherit;
    }
    body.dark .contact-form input,
    body.dark .contact-form textarea {
      background: #222;
      border-color: #3a3a3a;
      color: #eaeaea;
    }
    .contact-form textarea { min-height: 120px; }
    @media (max-width: 700px) { .contact-wrap { grid-template-columns: 1fr; } }

    /* ----- TESTIMONI ----- */
    .testi-grid {
      display: flex;
      gap: 1.5rem;
      overflow-x: auto;
      padding: 0.5rem 0.2rem 1.5rem;
      scroll-snap-type: x mandatory;
    }
    .testi-item {
      flex: 0 0 280px;
      background: white;
      padding: 1.5rem;
      border-radius: 24px;
      border: 1px solid #efefef;
      scroll-snap-align: start;
    }
    body.dark .testi-item { background: #1c1c1c; border-color: #2e2e2e; }
    .testi-item .stars { color: #f5b342; letter-spacing: 2px; }
    .testi-item img {
      width: 52px;
      height: 52px;
      border-radius: 50%;
      object-fit: cover;
      background: #ccc;
      margin-bottom: 0.5rem;
    }

    /* ----- FOOTER ----- */
    footer {
      border-top: 1px solid #eaeaea;
      padding: 2.5rem 0 1.5rem;
      margin-top: 2rem;
    }
    body.dark footer { border-top-color: #2a2a2a; }
    .footer-grid {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      gap: 2rem;
    }
    .footer-grid .col { flex: 1 1 160px; }
    .footer-grid .col a { display: block; margin: 0.3rem 0; }
    .back-top {
      display: inline-block;
      margin-top: 1.5rem;
      font-weight: 500;
    }

    /* animasi scroll */
    .fade-up {
      opacity: 0;
      transform: translateY(20px);
      transition: opacity 0.6s ease, transform 0.6s ease;
    }
    .fade-up.visible {
      opacity: 1;
      transform: translateY(0);
    }
  </style>
</head>
<body>
  <!-- NAVBAR -->
  <nav class="navbar" id="navbar">
    <div class="container">
      <div class="logo"><span>Dz</span>aka</div>
      <ul class="nav-menu" id="navMenu">
        <li><a href="#beranda" class="active">Beranda</a></li>
        <li><a href="#tentang">Tentang</a></li>
        <li><a href="#cv">CV</a></li>
        <li><a href="#karya">Hasil Karya</a></li>
        <li><a href="#fotoartikel">Foto & Artikel</a></li>
        <li><a href="#sosial">Media Sosial</a></li>
        <li><a href="#kontak">Kontak</a></li>
        <li><a href="#testimoni">Testimoni</a></li>
        <li><button class="theme-toggle" id="themeToggle"><i class="fas fa-moon"></i></button></li>
      </ul>
      <button class="hamburger" id="hamburger"><i class="fas fa-bars"></i></button>
    </div>
  </nav>

  <!-- LIGHTBOX -->
  <div class="lightbox-overlay" id="lightbox">
    <span class="lightbox-close" id="lightboxClose">&times;</span>
    <img id="lightboxImg" src="" alt="lightbox" />
  </div>

  <main>
    <!-- 1. BERANDA -->
    <section id="beranda" class="container fade-up">
      <div class="hero">
        <div class="hero-content">
          <h1>Halo, saya <br /><span style="color:#0b3b5c;">Dzaka Irfan Fadhilah</span></h1>
          <div class="subhead">UI/UX Designer & Pengembang Web</div>
          <p class="desc">Membangun pengalaman digital yang bermakna dengan kode dan desain. Fokus pada solusi elegan & responsif.</p>
          <div class="btn-group">
            <a href="#karya" class="btn btn-primary">Lihat Hasil Karya</a>
            <a href="#kontak" class="btn btn-outline">Hubungi Saya</a>
          </div>
          <div class="stats">
            <div class="stat-item"><span class="number">5+</span> <span class="label">Tahun pengalaman</span></div>
            <div class="stat-item"><span class="number">24</span> <span class="label">Proyek selesai</span></div>
            <div class="stat-item"><span class="number">12</span> <span class="label">Klien puas</span></div>
          </div>
        </div>
        <div class="hero-image">
          <img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='200' height='200' viewBox='0 0 100 100'%3E%3Ccircle cx='50' cy='50' r='45' fill='%23d9d9d9'/%3E%3Ctext x='50' y='55' font-size='20' text-anchor='middle' fill='%23555' font-family='Inter'%3E📸%3C/text%3E%3C/svg%3E" alt="Foto profil Dzaka" />
        </div>
      </div>
    </section>

    <!-- 2. TENTANG -->
    <section id="tentang" class="container fade-up">
      <h2 class="section-title">Tentang <span>Saya</span></h2>
      <div class="about-grid">
        <div class="about-image">
          <img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='400' height='300' viewBox='0 0 400 300'%3E%3Crect width='400' height='300' fill='%23e6e6e6'/%3E%3Ctext x='50' y='150' font-size='28' fill='%23555' font-family='Inter'%3E🖼️ Foto profil%3C/text%3E%3C/svg%3E" alt="Tentang Dzaka" />
        </div>
        <div class="about-text">
          <p><span class="highlight">Latar belakang:</span> Saya memulai karir sebagai desainer grafis, lalu beralih ke UI/UX dan pengembangan web. Menyukai kolaborasi lintas disiplin.</p>
          <p><span class="highlight">Visi & Misi:</span> Menciptakan antarmuka yang inklusif dan berkelanjutan. Setiap proyek adalah kesempatan untuk belajar dan tumbuh.</p>
          <p><span class="highlight">Keahlian:</span> Figma, React, Tailwind, PHP, dan desain sistem. Saya juga aktif menulis artikel tentang aksesibilitas.</p>
          <p><span class="highlight">Nilai:</span> Kejujuran, ketekunan, dan keberanian untuk bereksperimen.</p>
        </div>
      </div>
    </section>

    <!-- 3. CV -->
    <section id="cv" class="container fade-up">
      <h2 class="section-title">CV / <span>Resume</span></h2>
      <div class="cv-grid">
        <div class="cv-card"><h3>📘 Pendidikan</h3><div class="cv-item"><strong>S1 Informatika</strong> Universitas Brawijaya (2016-2020)</div></div>
        <div class="cv-card"><h3>💼 Pengalaman</h3><div class="cv-item"><strong>UI/UX Designer</strong> PT. Kreasi Digital (2021-sekarang)</div><div class="cv-item"><strong>Web Developer</strong> Freelance (2019-2021)</div></div>
        <div class="cv-card"><h3>🏅 Organisasi</h3><div class="cv-item">Ketua Divisi Desain · GDSC UB (2018-2019)</div></div>
        <div class="cv-card"><h3>⚡ Keahlian</h3><div>Figma, React, Tailwind, PHP, MySQL, UI/UX Research</div></div>
      </div>
      <div class="cv-timeline" style="margin-top:1.5rem;"><h3>📅 Timeline</h3><div class="cv-item"><span class="year">2021 - sekarang</span> · Designer di Kreasi Digital</div><div class="cv-item"><span class="year">2019 - 2021</span> · Freelance Web & Desain</div></div>
      <div class="download-cv"><a href="#" class="btn btn-primary"><i class="fas fa-download"></i> Download CV (PDF)</a></div>
    </section>

    <!-- 4. HASIL KARYA -->
    <section id="karya" class="container fade-up">
      <h2 class="section-title">Hasil <span>Karya</span></h2>
      <div class="filter-group">
        <button class="filter-btn active" data-filter="all">Semua</button>
        <button class="filter-btn" data-filter="desain">Desain</button>
        <button class="filter-btn" data-filter="foto">Fotografi</button>
        <button class="filter-btn" data-filter="video">Video</button>
        <button class="filter-btn" data-filter="web">Website</button>
      </div>
      <div class="portfolio-grid" id="portfolioGrid">
        <div class="portfolio-item" data-cat="desain"><img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='200' height='150' viewBox='0 0 200 150'%3E%3Crect fill='%23d9d9d9' width='200' height='150'/%3E%3Ctext x='30' y='80' fill='%23555' font-size='18'%3E🎨 Desain%3C/text%3E%3C/svg%3E" alt="proyek desain"><div class="portfolio-info"><h4>Brand Identity</h4><div class="category">Desain · 2025</div><a href="#" class="btn-small">Lihat Detail →</a></div></div>
        <div class="portfolio-item" data-cat="web"><img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='200' height='150' viewBox='0 0 200 150'%3E%3Crect fill='%23d9d9d9' width='200' height='150'/%3E%3Ctext x='30' y='80' fill='%23555' font-size='18'%3E🌐 Website%3C/text%3E%3C/svg%3E" alt="proyek web"><div class="portfolio-info"><h4>Landing Page Tech</h4><div class="category">Website · 2024</div><a href="#" class="btn-small">Lihat Detail →</a></div></div>
        <div class="portfolio-item" data-cat="foto"><img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='200' height='150' viewBox='0 0 200 150'%3E%3Crect fill='%23d9d9d9' width='200' height='150'/%3E%3Ctext x='30' y='80' fill='%23555' font-size='18'%3E📸 Foto%3C/text%3E%3C/svg%3E" alt="proyek foto"><div class="portfolio-info"><h4>Potret Urban</h4><div class="category">Fotografi · 2023</div><a href="#" class="btn-small">Lihat Detail →</a></div></div>
        <div class="portfolio-item" data-cat="video"><img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='200' height='150' viewBox='0 0 200 150'%3E%3Crect fill='%23d9d9d9' width='200' height='150'/%3E%3Ctext x='30' y='80' fill='%23555' font-size='18'%3E🎬 Video%3C/text%3E%3C/svg%3E" alt="proyek video"><div class="portfolio-info"><h4>Motion Reel</h4><div class="category">Video · 2025</div><a href="#" class="btn-small">Lihat Detail →</a></div></div>
      </div>
    </section>

    <!-- 5. FOTO & ARTIKEL -->
    <section id="fotoartikel" class="container fade-up">
      <h2 class="section-title">Foto & <span>Artikel</span></h2>
      <div class="photo-grid" id="photoGrid">
        <img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='200' height='200' viewBox='0 0 200 200'%3E%3Crect width='200' height='200' fill='%23ccc'/%3E%3Ctext x='60' y='110' fill='%23555' font-size='18'%3E📷 1%3C/text%3E%3C/svg%3E" alt="foto 1" onclick="openLightbox(this.src)" />
        <img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='200' height='200' viewBox='0 0 200 200'%3E%3Crect width='200' height='200' fill='%23bbb'/%3E%3Ctext x='60' y='110' fill='%23555' font-size='18'%3E📷 2%3C/text%3E%3C/svg%3E" alt="foto 2" onclick="openLightbox(this.src)" />
        <img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='200' height='200' viewBox='0 0 200 200'%3E%3Crect width='200' height='200' fill='%23ddd'/%3E%3Ctext x='60' y='110' fill='%23555' font-size='18'%3E📷 3%3C/text%3E%3C/svg%3E" alt="foto 3" onclick="openLightbox(this.src)" />
        <img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='200' height='200' viewBox='0 0 200 200'%3E%3Crect width='200' height='200' fill='%23c9c9c9'/%3E%3Ctext x='60' y='110' fill='%23555' font-size='18'%3E📷 4%3C/text%3E%3C/svg%3E" alt="foto 4" onclick="openLightbox(this.src)" />
      </div>
      <div class="article-grid">
        <div class="article-card"><img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/s
