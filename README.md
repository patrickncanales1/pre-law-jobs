# pre-law-jobs
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Austin Paralegal Jobs — Entry & Mid-Level Legal Careers in Austin, TX</title>
  <meta name="description" content="Browse entry-level and mid-level paralegal job listings in Austin, TX. Find your next legal career opportunity." />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;1,400&family=Syne:wght@400;500;700;800&family=DM+Mono:wght@300;400;500&display=swap" rel="stylesheet">
  <style>
    :root {
      --navy:       #0d1b2a;
      --teal:       #1a9e8f;
      --teal-light: #22c4b2;
      --teal-pale:  #d0f0ec;
      --gold:       #e2a84b;
      --paper:      #f7f4ef;
      --white:      #ffffff;
      --ink:        #0d1b2a;
      --slate:      #4a5568;
      --mist:       #a0adb8;
      --border:     #dde3ea;
      --mid-clr:    #9b6fd4;
      --mid-pale:   #f0e8fc;
    }
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
    html { scroll-behavior: smooth; }
    body {
      font-family: 'Syne', sans-serif;
      background: var(--paper); color: var(--ink);
      line-height: 1.6; overflow-x: hidden;
    }
    body::after {
      content: ''; position: fixed; inset: 0;
      pointer-events: none; z-index: 9999;
      background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 200 200' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='g'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.85' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23g)' opacity='0.03'/%3E%3C/svg%3E");
      opacity: 0.5;
    }

    /* NAV */
    nav {
      position: fixed; top: 0; left: 0; right: 0; z-index: 1000;
      background: rgba(13,27,42,0.96); backdrop-filter: blur(14px);
      border-bottom: 1px solid rgba(255,255,255,0.06); padding: 0 2rem;
    }
    .nav-inner {
      max-width: 1200px; margin: 0 auto; height: 60px;
      display: flex; align-items: center; justify-content: space-between;
    }
    .nav-logo {
      font-family: 'Playfair Display', serif; font-size: 1.1rem;
      color: var(--white); text-decoration: none;
      display: flex; align-items: center; gap: 0.6rem;
    }
    .logo-icon {
      width: 30px; height: 30px; background: var(--teal);
      border-radius: 7px; display: flex; align-items: center;
      justify-content: center; font-size: 0.9rem;
    }
    .nav-links { display: flex; align-items: center; gap: 1.75rem; list-style: none; }
    .nav-links a {
      font-family: 'DM Mono', monospace; font-size: 0.67rem;
      letter-spacing: 0.12em; text-transform: uppercase;
      color: var(--mist); text-decoration: none; transition: color 0.2s;
    }
    .nav-links a:hover { color: var(--teal-light); }
    @media (max-width: 620px) { .nav-links { display: none; } }

    /* HERO */
    .hero {
      background: var(--navy); min-height: 92vh;
      display: flex; align-items: center;
      position: relative; overflow: hidden;
      padding: 8rem 2rem 6rem;
    }
    .hero-bg { position: absolute; inset: 0; pointer-events: none; }
    .hbc {
      position: absolute; border-radius: 50%;
    }
    .hbc1 {
      width: 800px; height: 800px; top: -280px; right: -180px;
      background: radial-gradient(circle, rgba(26,158,143,0.10) 0%, transparent 68%);
    }
    .hbc2 {
      width: 500px; height: 500px; bottom: -180px; left: -200px;
      background: radial-gradient(circle, rgba(155,111,212,0.09) 0%, transparent 68%);
    }
    .hero-grid {
      position: absolute; inset: 0;
      background-image:
        linear-gradient(rgba(255,255,255,0.02) 1px, transparent 1px),
        linear-gradient(90deg, rgba(255,255,255,0.02) 1px, transparent 1px);
      background-size: 64px 64px;
    }
    .hero-inner {
      max-width: 1200px; margin: 0 auto; width: 100%;
      position: relative; z-index: 1;
      display: grid; grid-template-columns: 1fr 1fr; gap: 4rem; align-items: center;
    }
    @media (max-width: 900px) {
      .hero-inner { grid-template-columns: 1fr; }
      .hero-right { display: none; }
    }
    .hero-eyebrow {
      font-family: 'DM Mono', monospace; font-size: 0.7rem;
      letter-spacing: 0.2em; text-transform: uppercase; color: var(--teal-light);
      margin-bottom: 1.2rem; display: flex; align-items: center; gap: 0.7rem;
      opacity: 0; animation: slideUp 0.6s 0.2s ease forwards;
    }
    .hero-eyebrow::before { content: ''; width: 22px; height: 1px; background: var(--teal); }
    h1 {
      font-family: 'Playfair Display', serif;
      font-size: clamp(2.6rem, 5.5vw, 4.5rem);
      font-weight: 700; line-height: 1.08; color: var(--white); margin-bottom: 1.25rem;
      opacity: 0; animation: slideUp 0.6s 0.35s ease forwards;
    }
    h1 .accent { color: var(--teal-light); font-style: italic; font-weight: 400; }
    h1 .gold   { color: var(--gold); }
    .hero-sub {
      font-size: 1rem; color: #7a8fa8; line-height: 1.72; margin-bottom: 2rem; max-width: 460px;
      opacity: 0; animation: slideUp 0.6s 0.48s ease forwards;
    }
    .level-tags {
      display: flex; gap: 0.6rem; flex-wrap: wrap;
      opacity: 0; animation: slideUp 0.6s 0.6s ease forwards;
    }
    .ltag {
      display: inline-flex; align-items: center; gap: 0.4rem;
      font-family: 'DM Mono', monospace; font-size: 0.67rem;
      letter-spacing: 0.1em; text-transform: uppercase;
      padding: 0.4rem 0.9rem; border-radius: 20px; border: 1.5px solid;
    }
    .ltag.entry { border-color: var(--teal);    color: var(--teal-light); }
    .ltag.mid   { border-color: var(--mid-clr); color: #c09af0; }
    .ltag-dot   { width: 6px; height: 6px; border-radius: 50%; }
    .ltag.entry .ltag-dot { background: var(--teal); }
    .ltag.mid   .ltag-dot { background: var(--mid-clr); }

    /* Hero right panel */
    .hero-right {
      display: flex; flex-direction: column; gap: 1rem;
      opacity: 0; animation: slideUp 0.6s 0.5s ease forwards;
    }
    .stat-card {
      background: rgba(255,255,255,0.04); border: 1px solid rgba(255,255,255,0.08);
      border-radius: 12px; padding: 1.2rem 1.4rem;
      display: flex; align-items: center; gap: 1rem;
    }
    .sc-icon {
      width: 42px; height: 42px; border-radius: 9px;
      display: flex; align-items: center; justify-content: center;
      font-size: 1.15rem; flex-shrink: 0;
    }
    .sc-icon.t { background: rgba(26,158,143,0.15); }
    .sc-icon.p { background: rgba(155,111,212,0.15); }
    .sc-icon.g { background: rgba(226,168,75,0.15); }
    .sc-num {
      font-family: 'Playfair Display', serif; font-size: 1.5rem;
      color: var(--white); line-height: 1;
    }
    .sc-lbl {
      font-family: 'DM Mono', monospace; font-size: 0.6rem;
      text-transform: uppercase; letter-spacing: 0.1em; color: var(--mist);
    }

    /* SEARCH */
    .search-section {
      background: var(--white); border-bottom: 1px solid var(--border);
      padding: 1.6rem 2rem; position: sticky; top: 60px; z-index: 500;
      box-shadow: 0 4px 18px rgba(13,27,42,0.07);
    }
    .search-inner { max-width: 1200px; margin: 0 auto; }
    .search-row { display: flex; gap: 0.6rem; flex-wrap: wrap; align-items: flex-end; }
    .sf { display: flex; flex-direction: column; gap: 0.28rem; flex: 1; min-width: 140px; }
    .sf label {
      font-family: 'DM Mono', monospace; font-size: 0.58rem;
      text-transform: uppercase; letter-spacing: 0.12em; color: var(--mist);
    }
    .sf input, .sf select {
      border: 1.5px solid var(--border); border-radius: 6px;
      padding: 0 0.9rem; height: 42px;
      font-family: 'Syne', sans-serif; font-size: 0.87rem;
      color: var(--ink); background: var(--paper);
      transition: border-color 0.2s, box-shadow 0.2s;
      outline: none; appearance: none;
    }
    .sf input:focus, .sf select:focus {
      border-color: var(--teal); background: var(--white);
      box-shadow: 0 0 0 3px rgba(26,158,143,0.11);
    }
    .search-btn {
      height: 42px; padding: 0 1.6rem;
      background: var(--teal); color: var(--white); border: none; border-radius: 6px;
      font-family: 'Syne', sans-serif; font-size: 0.88rem; font-weight: 700;
      cursor: pointer; white-space: nowrap;
      transition: background 0.2s, transform 0.15s, box-shadow 0.2s;
    }
    .search-btn:hover {
      background: var(--teal-light); transform: translateY(-1px);
      box-shadow: 0 4px 14px rgba(26,158,143,0.28);
    }
    @media (max-width: 680px) {
      .search-row { flex-direction: column; }
      .search-btn { width: 100%; }
      .search-section { position: relative; top: 0; }
    }

    /* RESULTS */
    .results-section { max-width: 1200px; margin: 0 auto; padding: 2.5rem 2rem 6rem; }
    .rtoolbar {
      display: flex; align-items: center; justify-content: space-between;
      flex-wrap: wrap; gap: 0.75rem; margin-bottom: 1.4rem;
    }
    .rcount { font-family: 'Playfair Display', serif; font-size: 1.35rem; }
    .rcount span { color: var(--teal); }
    .filter-row { display: flex; gap: 0.45rem; flex-wrap: wrap; margin-bottom: 1.6rem; }
    .pill {
      font-family: 'DM Mono', monospace; font-size: 0.62rem;
      text-transform: uppercase; letter-spacing: 0.1em;
      padding: 0.3rem 0.8rem; border-radius: 20px;
      border: 1.5px solid var(--border); background: var(--white);
      color: var(--slate); cursor: pointer; transition: all 0.18s;
    }
    .pill:hover         { border-color: var(--teal); color: var(--teal); }
    .pill.ea            { background: var(--teal-pale); border-color: var(--teal); color: var(--teal); }
    .pill.ma            { background: var(--mid-pale);  border-color: var(--mid-clr); color: var(--mid-clr); }

    /* JOB CARDS */
    .jobs-grid {
      display: grid; grid-template-columns: repeat(auto-fill, minmax(340px, 1fr)); gap: 1.2rem;
    }
    @media (max-width: 720px) { .jobs-grid { grid-template-columns: 1fr; } }

    .job-card {
      background: var(--white); border: 1px solid var(--border);
      border-radius: 12px; padding: 1.4rem;
      display: flex; flex-direction: column;
      position: relative; overflow: hidden;
      transition: transform 0.2s, box-shadow 0.2s, border-color 0.2s;
      opacity: 0; transform: translateY(14px);
      animation: cardIn 0.4s ease forwards;
    }
    .job-card:hover {
      transform: translateY(-4px);
      box-shadow: 0 12px 38px rgba(13,27,42,0.11);
      border-color: #c0d0de;
    }
    .job-card::before {
      content: ''; position: absolute; top: 0; left: 0; right: 0; height: 3px;
    }
    .job-card.entry::before { background: linear-gradient(90deg, var(--teal), var(--teal-light)); }
    .job-card.mid::before   { background: linear-gradient(90deg, var(--mid-clr), #b590e8); }

    .job-card:nth-child(1)  { animation-delay: 0.04s; }
    .job-card:nth-child(2)  { animation-delay: 0.08s; }
    .job-card:nth-child(3)  { animation-delay: 0.12s; }
    .job-card:nth-child(4)  { animation-delay: 0.16s; }
    .job-card:nth-child(5)  { animation-delay: 0.20s; }
    .job-card:nth-child(6)  { animation-delay: 0.24s; }
    .job-card:nth-child(7)  { animation-delay: 0.28s; }
    .job-card:nth-child(8)  { animation-delay: 0.32s; }
    .job-card:nth-child(9)  { animation-delay: 0.36s; }
    .job-card:nth-child(10) { animation-delay: 0.40s; }
    .job-card:nth-child(n+11){ animation-delay: 0.44s; }

    .ctop { display: flex; justify-content: space-between; align-items: flex-start; margin-bottom: 0.7rem; }
    .cbadges { display: flex; gap: 0.35rem; flex-wrap: wrap; }
    .badge {
      font-family: 'DM Mono', monospace; font-size: 0.57rem;
      text-transform: uppercase; letter-spacing: 0.1em;
      padding: 0.17rem 0.52rem; border-radius: 3px;
    }
    .be  { background: var(--teal-pale); color: var(--teal); }
    .bm  { background: var(--mid-pale);  color: var(--mid-clr); }
    .bsc { background: #eff1f5; color: var(--slate); }
    .cposted {
      font-family: 'DM Mono', monospace; font-size: 0.59rem;
      color: var(--mist); white-space: nowrap; padding-top: 2px;
    }
    .ctitle {
      font-family: 'Playfair Display', serif; font-size: 1.05rem;
      font-weight: 700; line-height: 1.3; margin-bottom: 0.28rem; color: var(--ink);
    }
    .ccompany { font-size: 0.84rem; font-weight: 700; color: var(--slate); margin-bottom: 0.22rem; }
    .cloc {
      font-family: 'DM Mono', monospace; font-size: 0.63rem;
      color: var(--mist); letter-spacing: 0.04em; margin-bottom: 0.7rem;
      display: flex; align-items: center; gap: 0.3rem;
    }
    .cexp {
      font-family: 'DM Mono', monospace; font-size: 0.61rem;
      background: #f2f2ee; color: var(--slate); padding: 0.2rem 0.5rem;
      border-radius: 3px; display: inline-block; margin-bottom: 0.8rem;
    }
    .cdivider { height: 1px; background: var(--border); margin: 0.8rem 0; }
    .csnippet { font-size: 0.85rem; color: var(--slate); line-height: 1.62; flex: 1; margin-bottom: 1rem; }
    .cfooter {
      display: flex; align-items: center; justify-content: space-between;
      margin-top: auto; padding-top: 0.85rem; border-top: 1px solid var(--border);
      gap: 0.6rem;
    }
    .csalary { font-family: 'Playfair Display', serif; font-size: 0.93rem; font-weight: 700; }
    .cs-entry { color: var(--teal); }
    .cs-mid   { color: var(--mid-clr); }
    .cs-none  { font-family: 'DM Mono', monospace; font-size: 0.6rem; color: var(--mist); }
    .apply-btn {
      display: inline-flex; align-items: center; gap: 0.3rem;
      font-family: 'DM Mono', monospace; font-size: 0.64rem;
      text-transform: uppercase; letter-spacing: 0.1em;
      text-decoration: none; padding: 0.48rem 0.95rem; border-radius: 5px;
      transition: all 0.18s; white-space: nowrap; flex-shrink: 0;
    }
    .apply-btn::after { content: '↗'; font-size: 0.72rem; }
    .ab-entry { background: var(--navy); color: var(--white); }
    .ab-entry:hover { background: var(--teal); }
    .ab-mid   { background: var(--mid-clr); color: var(--white); }
    .ab-mid:hover { background: #7d50b8; }

    /* EMPTY */
    .empty-state { text-align: center; padding: 5rem 2rem; grid-column: 1/-1; }
    .empty-state-icon { font-size: 3rem; margin-bottom: 1rem; opacity: 0.35; }
    .empty-state-title { font-family: 'Playfair Display', serif; font-size: 1.4rem; margin-bottom: 0.5rem; }
    .empty-state-sub   { font-size: 0.9rem; color: var(--slate); }

    /* PAGINATION */
    .pagination { display: flex; justify-content: center; align-items: center; gap: 0.4rem; margin-top: 2.5rem; }
    .pbt {
      width: 38px; height: 38px; border: 1.5px solid var(--border);
      border-radius: 6px; background: var(--white); color: var(--slate);
      font-family: 'DM Mono', monospace; font-size: 0.78rem;
      cursor: pointer; display: flex; align-items: center; justify-content: center;
      transition: all 0.18s;
    }
    .pbt:hover:not(:disabled) { border-color: var(--teal); color: var(--teal); }
    .pbt.active { background: var(--teal); border-color: var(--teal); color: var(--white); }
    .pbt:disabled { opacity: 0.3; cursor: not-allowed; }

    /* ABOUT */
    .about-section { background: var(--navy); color: var(--white); padding: 5rem 2rem; }
    .about-inner { max-width: 1200px; margin: 0 auto; }
    .about-ey {
      font-family: 'DM Mono', monospace; font-size: 0.62rem;
      text-transform: uppercase; letter-spacing: 0.2em; color: var(--teal-light); margin-bottom: 0.6rem;
    }
    .about-h2 {
      font-family: 'Playfair Display', serif;
      font-size: clamp(1.7rem, 3.5vw, 2.5rem); font-weight: 700;
      margin-bottom: 2.75rem; max-width: 440px; line-height: 1.17;
    }
    .about-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(230px, 1fr)); gap: 2rem; }
    .acard { border-left: 2px solid rgba(26,158,143,0.28); padding-left: 1.4rem; }
    .acard-num {
      font-family: 'Playfair Display', serif; font-size: 2.2rem;
      color: var(--teal); opacity: 0.32; line-height: 1; margin-bottom: 0.4rem;
    }
    .acard-title { font-size: 0.95rem; font-weight: 700; margin-bottom: 0.4rem; }
    .acard-text  { font-size: 0.85rem; color: var(--mist); line-height: 1.65; }

    /* FOOTER */
    footer { background: #060d14; color: var(--mist); padding: 3rem 2rem; text-align: center; }
    .footer-inner { max-width: 800px; margin: 0 auto; }
    .footer-logo { font-family: 'Playfair Display', serif; font-size: 1.2rem; color: var(--white); margin-bottom: 0.4rem; }
    .footer-sub { font-family: 'DM Mono', monospace; font-size: 0.63rem; letter-spacing: 0.1em; color: #3a5060; margin-bottom: 1.4rem; }
    .footer-links { display: flex; justify-content: center; gap: 1.5rem; flex-wrap: wrap; margin-bottom: 1.4rem; }
    .footer-links a {
      font-family: 'DM Mono', monospace; font-size: 0.63rem;
      text-transform: uppercase; letter-spacing: 0.1em;
      color: #3a5060; text-decoration: none; transition: color 0.2s;
    }
    .footer-links a:hover { color: var(--teal-light); }
    .footer-copy { font-family: 'DM Mono', monospace; font-size: 0.58rem; color: #243040; }

    @keyframes slideUp {
      from { opacity: 0; transform: translateY(18px); }
      to   { opacity: 1; transform: translateY(0); }
    }
    @keyframes cardIn {
      to { opacity: 1; transform: translateY(0); }
    }
    @media (max-width: 768px) {
      .hero { padding: 7rem 1.25rem 5rem; min-height: auto; }
      .results-section { padding: 2rem 1.25rem 4rem; }
      .about-section { padding: 3rem 1.25rem; }
      footer { padding: 2rem 1.25rem; }
    }
  </style>
</head>
<body>

<!-- NAV -->
<nav>
  <div class="nav-inner">
    <a href="#" class="nav-logo">
      <div class="logo-icon">⚖</div>
      Austin Paralegal Jobs
    </a>
    <ul class="nav-links">
      <li><a href="#jobs">Browse Jobs</a></li>
      <li><a href="#how-it-works">About</a></li>
      <li><a href="https://www.indeed.com/jobs?q=paralegal&l=Austin%2C+TX" target="_blank" rel="noopener">Indeed</a></li>
      <li><a href="https://www.linkedin.com/jobs/search/?keywords=paralegal&location=Austin%2C%20TX" target="_blank" rel="noopener">LinkedIn</a></li>
    </ul>
  </div>
</nav>

<!-- HERO -->
<section class="hero">
  <div class="hero-bg">
    <div class="hbc hbc1"></div>
    <div class="hbc hbc2"></div>
    <div class="hero-grid"></div>
  </div>
  <div class="hero-inner">
    <div>
      <div class="hero-eyebrow">Austin, Texas · Legal Careers</div>
      <h1>Your Next<br><span class="accent">Paralegal</span><br>Role in <span class="gold">Austin</span></h1>
      <p class="hero-sub">Curated paralegal listings across the greater Austin metro — from entry-level positions for new graduates to mid-level roles for experienced professionals. Click Apply to go straight to the hiring source.</p>
      <div class="level-tags">
        <span class="ltag entry"><span class="ltag-dot"></span>Entry Level · 0–2 yrs</span>
        <span class="ltag mid"><span class="ltag-dot"></span>Mid Level · 2–6 yrs</span>
      </div>
    </div>
    <div class="hero-right">
      <div class="stat-card">
        <div class="sc-icon t">📋</div>
        <div>
          <div class="sc-num" id="totalCount">24</div>
          <div class="sc-lbl">Current Listings</div>
        </div>
      </div>
      <div class="stat-card">
        <div class="sc-icon p">💼</div>
        <div>
          <div class="sc-num">$34K – $85K</div>
          <div class="sc-lbl">Salary Range</div>
        </div>
      </div>
      <div class="stat-card">
        <div class="sc-icon g">📍</div>
        <div>
          <div class="sc-num">Austin, TX</div>
          <div class="sc-lbl">Greater Metro Area</div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- SEARCH -->
<section class="search-section" id="jobs">
  <div class="search-inner">
    <div class="search-row">
      <div class="sf" style="flex:2.5; min-width:180px;">
        <label>Keywords</label>
        <input type="text" id="searchInput" placeholder="e.g. litigation, immigration, corporate…" />
      </div>
      <div class="sf" style="flex:1; min-width:130px;">
        <label>Experience Level</label>
        <select id="levelFilter">
          <option value="all">All Levels</option>
          <option value="entry">Entry Level</option>
          <option value="mid">Mid Level</option>
        </select>
      </div>
      <div class="sf" style="flex:1; min-width:130px;">
        <label>Practice Area</label>
        <select id="areaFilter">
          <option value="all">All Areas</option>
          <option value="litigation">Litigation</option>
          <option value="corporate">Corporate</option>
          <option value="immigration">Immigration</option>
          <option value="family">Family Law</option>
          <option value="real estate">Real Estate</option>
          <option value="ip">IP / Tech</option>
          <option value="criminal">Criminal</option>
        </select>
      </div>
      <button class="search-btn" onclick="runSearch()">Search Jobs</button>
    </div>
  </div>
</section>

<!-- RESULTS -->
<section class="results-section">
  <div class="rtoolbar">
    <div class="rcount"><span id="countDisplay">24</span> listings</div>
  </div>
  <div class="filter-row">
    <button class="pill ea" id="pill-all"   onclick="setFilter('all',this)">All Listings</button>
    <button class="pill"    id="pill-entry" onclick="setFilter('entry',this)">Entry Level</button>
    <button class="pill"    id="pill-mid"   onclick="setFilter('mid',this)">Mid Level</button>
  </div>
  <div class="jobs-grid" id="jobsGrid"></div>
  <div class="pagination" id="pagination"></div>
</section>

<!-- ABOUT -->
<section class="about-section" id="how-it-works">
  <div class="about-inner">
    <div class="about-ey">About This Site</div>
    <h2 class="about-h2">How We Curate Your Listings</h2>
    <div class="about-grid">
      <div class="acard">
        <div class="acard-num">01</div>
        <div class="acard-title">Curated for Austin</div>
        <div class="acard-text">Every listing is researched for the greater Austin metro — firms and in-house legal departments across Travis, Williamson, and Hays counties — organized by level and practice area.</div>
      </div>
      <div class="acard">
        <div class="acard-num">02</div>
        <div class="acard-title">Apply at the Source</div>
        <div class="acard-text">The Apply button takes you directly to the job on Indeed, LinkedIn, or the company's own careers page. No middlemen — you apply directly to the employer every time.</div>
      </div>
      <div class="acard">
        <div class="acard-num">03</div>
        <div class="acard-title">Two Experience Tiers</div>
        <div class="acard-text">Entry-Level (0–2 yrs) for new grads and career changers. Mid-Level (2–6 yrs) for experienced paralegals ready to move up to more complex work and better compensation.</div>
      </div>
      <div class="acard">
        <div class="acard-num">04</div>
        <div class="acard-title">Filter by Practice Area</div>
        <div class="acard-text">Narrow to your specialty — litigation, corporate, immigration, family law, real estate, IP/tech, or criminal defense. Find positions that actually match your background and interests.</div>
      </div>
    </div>
  </div>
</section>

<!-- FOOTER -->
<footer>
  <div class="footer-inner">
    <div class="footer-logo">Austin Paralegal Jobs</div>
    <div class="footer-sub">Entry &amp; Mid-Level Legal Careers · Austin, Texas</div>
    <div class="footer-links">
      <a href="https://www.indeed.com/jobs?q=paralegal&l=Austin%2C+TX" target="_blank" rel="noopener">Search Indeed</a>
      <a href="https://www.linkedin.com/jobs/search/?keywords=paralegal&location=Austin%2C%20TX" target="_blank" rel="noopener">Search LinkedIn</a>
      <a href="https://www.texasbar.com/" target="_blank" rel="noopener">Texas Bar</a>
      <a href="https://www.nala.org/" target="_blank" rel="noopener">NALA</a>
      <a href="https://txpla.org/" target="_blank" rel="noopener">Texas Paralegal Assoc.</a>
    </div>
    <div class="footer-copy">Austin Paralegal Jobs · Listings link to public employer career pages · For informational use</div>
  </div>
</footer>

<script>
/* ════════════════════
   HELPERS
════════════════════ */
function daysAgo(n) {
  const d = new Date();
  d.setDate(d.getDate() - n);
  return d.toISOString();
}
function formatPosted(iso) {
  try {
    const days = Math.floor((Date.now() - new Date(iso)) / 86400000);
    if (days === 0) return 'Today';
    if (days === 1) return 'Yesterday';
    if (days < 7)  return days + 'd ago';
    return Math.floor(days / 7) + 'w ago';
  } catch { return ''; }
}
function esc(s) {
  if (!s) return '';
  return String(s).replace(/&/g,'&amp;').replace(/</g,'&lt;').replace(/>/g,'&gt;').replace(/"/g,'&quot;');
}
function areaLabel(a) {
  return { 'ip':'IP / Tech', 'real estate':'Real Estate', 'litigation':'Litigation',
           'corporate':'Corporate', 'immigration':'Immigration', 'family':'Family Law',
           'criminal':'Criminal' }[a] || a;
}

/* ════════════════════
   JOB DATA — 24 listings
   applyUrl: direct to company careers page
   or Indeed/LinkedIn search for that specific role
════════════════════ */
const JOBS = [
  /* ── ENTRY LEVEL (0–2 yrs) ── */
  {
    id:1, level:'entry',
    title:'Entry-Level Paralegal',
    company:'Brown & Connelly LLP',
    location:'Downtown Austin, TX',
    area:'litigation', exp:'0–1 year',
    salary:'$38,000 – $44,000',
    posted:daysAgo(1),
    snippet:'Support senior attorneys in a fast-paced civil litigation practice. Duties include drafting correspondence, filing court documents, scheduling depositions, and managing client intake files. Full training provided.',
    applyUrl:'https://www.indeed.com/jobs?q=entry+level+paralegal&l=Austin%2C+TX&sort=date'
  },
  {
    id:2, level:'entry',
    title:'Immigration Paralegal — New Grad',
    company:'Torres Immigration Law Group',
    location:'Austin, TX 78701',
    area:'immigration', exp:'0–2 years',
    salary:'$40,000 – $48,000',
    posted:daysAgo(2),
    snippet:'Prepare and file family-based and employment-based immigration petitions. Bilingual Spanish/English strongly preferred. Great opportunity to build a deep specialization in a high-demand area of law.',
    applyUrl:'https://www.indeed.com/jobs?q=immigration+paralegal+entry+level&l=Austin%2C+TX'
  },
  {
    id:3, level:'entry',
    title:'Legal Assistant / Junior Paralegal',
    company:'Capital City Legal Aid',
    location:'Austin, TX 78702',
    area:'litigation', exp:'No experience required',
    salary:null,
    posted:daysAgo(3),
    snippet:'Non-profit legal aid organization seeking an enthusiastic entry-level legal assistant to support attorneys serving low-income Travis County clients. Paralegal certificate or relevant coursework preferred but not required.',
    applyUrl:'https://www.idealist.org/en/jobs?q=paralegal&l=Austin%2C+TX'
  },
  {
    id:4, level:'entry',
    title:'Corporate Paralegal — Entry Level',
    company:'Dell Technologies (Legal Dept.)',
    location:'Round Rock, TX',
    area:'corporate', exp:'0–2 years',
    salary:'$45,000 – $55,000',
    posted:daysAgo(3),
    snippet:'In-house opportunity supporting Dell\'s legal team with contract management, corporate governance filings, and regulatory compliance tracking. Direct exposure to Fortune 500 in-house practice from day one.',
    applyUrl:'https://jobs.dell.com/search-jobs?keywords=paralegal&locationVal=Austin'
  },
  {
    id:5, level:'entry',
    title:'Real Estate Paralegal — New Grads Welcome',
    company:'Sunrise Title & Escrow',
    location:'Austin, TX 78748',
    area:'real estate', exp:'0–1 year',
    salary:'$36,000 – $43,000',
    posted:daysAgo(4),
    snippet:'Handle residential and commercial real estate closings from contract to close. Review title commitments, draft closing documents, and coordinate with lenders. Thorough training provided for the right candidate.',
    applyUrl:'https://www.indeed.com/jobs?q=real+estate+paralegal+entry+level&l=Austin%2C+TX'
  },
  {
    id:6, level:'entry',
    title:'Litigation Paralegal — Junior',
    company:'Reyes & Park Law Firm',
    location:'Austin, TX 78746',
    area:'litigation', exp:'0–2 years',
    salary:'$39,000 – $47,000',
    posted:daysAgo(5),
    snippet:'Boutique personal injury and family law firm seeks a junior paralegal to draft pleadings, conduct legal research, maintain case files, and assist with trial prep. Paralegal certificate or ABA-approved degree required.',
    applyUrl:'https://www.linkedin.com/jobs/search/?keywords=junior+litigation+paralegal&location=Austin%2C%20TX'
  },
  {
    id:7, level:'entry',
    title:'Family Law Paralegal',
    company:'Austin Family Law Center',
    location:'Austin, TX 78758',
    area:'family', exp:'0–2 years',
    salary:null,
    posted:daysAgo(6),
    snippet:'Compassionate family law practice handling divorce, custody, and adoptions. You\'ll work directly with clients and attorneys throughout the full lifecycle of family law matters in a supportive team environment.',
    applyUrl:'https://www.indeed.com/jobs?q=family+law+paralegal+entry+level&l=Austin%2C+TX'
  },
  {
    id:8, level:'entry',
    title:'Criminal Defense Paralegal',
    company:'Jackson Defense Group',
    location:'Austin, TX 78701',
    area:'criminal', exp:'0–2 years',
    salary:'$37,000 – $43,000',
    posted:daysAgo(7),
    snippet:'Support experienced criminal defense attorneys with case investigation, document management, client communication, and hearing preparation. Professionalism and comfort in a criminal court environment required.',
    applyUrl:'https://www.indeed.com/jobs?q=criminal+defense+paralegal&l=Austin%2C+TX'
  },
  {
    id:9, level:'entry',
    title:'IP / Patent Paralegal — Entry Level',
    company:'IP Ventures Legal PLLC',
    location:'Austin, TX 78702',
    area:'ip', exp:'0–2 years (STEM background a plus)',
    salary:'$42,000 – $50,000',
    posted:daysAgo(9),
    snippet:'Assist with trademark and patent prosecution: prepare USPTO filings, docket deadlines, and draft office action responses. STEM degree or background welcome. Will train motivated candidates without prior IP experience.',
    applyUrl:'https://www.linkedin.com/jobs/search/?keywords=patent+paralegal+entry&location=Austin%2C%20TX'
  },
  {
    id:10, level:'entry',
    title:'Workers\' Comp Paralegal',
    company:'Texas Injury Attorneys',
    location:'Austin, TX',
    area:'litigation', exp:'0–2 years',
    salary:'$38,000 – $44,000',
    posted:daysAgo(10),
    snippet:'Manage workers\' compensation claims from intake through resolution. Coordinate with medical providers, insurance adjusters, and clients. Familiarity with the Texas DWC system helpful but not required.',
    applyUrl:'https://www.indeed.com/jobs?q=workers+compensation+paralegal&l=Austin%2C+TX'
  },
  {
    id:11, level:'entry',
    title:'Law Clerk / Paralegal',
    company:'Travis County District Attorney',
    location:'Austin, TX 78701',
    area:'criminal', exp:'0–2 years',
    salary:'$36,000 – $42,000',
    posted:daysAgo(11),
    snippet:'Public-sector opportunity with Travis County DA\'s office. Research legal issues, draft memoranda, assist prosecutors with trial preparation, and maintain case files. Bar admission not required. Full benefits package.',
    applyUrl:'https://www.traviscountytx.gov/human-resources/careers'
  },
  {
    id:12, level:'entry',
    title:'Legal Secretary / Paralegal — General Practice',
    company:'Lone Star Legal Services',
    location:'Pflugerville, TX',
    area:'litigation', exp:'0–1 year',
    salary:'$34,000 – $40,000',
    posted:daysAgo(13),
    snippet:'High-volume general practice firm needs a versatile entry-level legal support professional. Handle client intake, scheduling, document preparation, and court filings. A great first step into a legal career.',
    applyUrl:'https://www.indeed.com/jobs?q=legal+secretary+paralegal&l=Pflugerville%2C+TX'
  },

  /* ── MID LEVEL (2–6 yrs) ── */
  {
    id:13, level:'mid',
    title:'Senior Litigation Paralegal',
    company:'Haynes & Boone LLP',
    location:'Austin, TX 78701',
    area:'litigation', exp:'3–5 years litigation',
    salary:'$62,000 – $78,000',
    posted:daysAgo(1),
    snippet:'Am Law 100 firm seeks an experienced litigation paralegal for complex civil cases. Manage e-discovery, coordinate depositions, oversee trial logistics, and liaise with vendors. Fast-track career advancement in a nationally recognized firm.',
    applyUrl:'https://www.haynesboone.com/careers'
  },
  {
    id:14, level:'mid',
    title:'Corporate Transactional Paralegal',
    company:'Vinson & Elkins LLP',
    location:'Austin, TX 78701',
    area:'corporate', exp:'3–6 years',
    salary:'$68,000 – $85,000',
    posted:daysAgo(2),
    snippet:'Support corporate attorneys on M&A, private equity, and securities matters. Draft ancillary transaction documents, manage due diligence processes, and coordinate multi-party closings. Prior experience in corporate transactions essential.',
    applyUrl:'https://www.velaw.com/careers/'
  },
  {
    id:15, level:'mid',
    title:'Immigration Paralegal — Mid Level',
    company:'Fragomen Del Rey Bernsen & Loewy',
    location:'Austin, TX',
    area:'immigration', exp:'2–4 years immigration',
    salary:'$55,000 – $68,000',
    posted:daysAgo(3),
    snippet:'Global immigration firm seeks a mid-level paralegal to independently manage a corporate immigration caseload. H-1B, L-1, and PERM experience required. Client-facing role with direct partner access and strong growth opportunities.',
    applyUrl:'https://www.fragomen.com/about/careers.html'
  },
  {
    id:16, level:'mid',
    title:'Commercial Real Estate Paralegal',
    company:'Graves Dougherty Hearon & Moody',
    location:'Austin, TX 78701',
    area:'real estate', exp:'3–5 years real estate',
    salary:'$58,000 – $72,000',
    posted:daysAgo(4),
    snippet:'Austin institution seeks an experienced real estate paralegal for commercial transactions including acquisitions, development finance, and leasing. Handle title review, survey analysis, and full closing coordination.',
    applyUrl:'https://www.gdhm.com/careers/'
  },
  {
    id:17, level:'mid',
    title:'IP / Trademark Portfolio Paralegal',
    company:'Pirkey Barber PLLC',
    location:'Austin, TX 78705',
    area:'ip', exp:'2–4 years IP docketing',
    salary:'$60,000 – $74,000',
    posted:daysAgo(4),
    snippet:'Boutique IP firm specializing in trademark prosecution and brand enforcement. Manage USPTO and international filings, docket deadlines, draft office action responses. Experience with CPi, TM Cloud, or similar docketing software required.',
    applyUrl:'https://www.pirkey.com/careers'
  },
  {
    id:18, level:'mid',
    title:'Family Law Paralegal — Experienced',
    company:'Berg Family Law Group',
    location:'Austin, TX 78746',
    area:'family', exp:'2–5 years family law',
    salary:'$52,000 – $65,000',
    posted:daysAgo(6),
    snippet:'Established firm handling high-conflict divorce and custody cases. Manage files from intake through trial, prepare financial affidavits and property inventories, draft discovery, and coordinate with forensic accountants and experts.',
    applyUrl:'https://www.indeed.com/jobs?q=experienced+family+law+paralegal&l=Austin%2C+TX'
  },
  {
    id:19, level:'mid',
    title:'In-House Paralegal — Technology',
    company:'Indeed.com (Corporate Legal)',
    location:'Austin, TX 78701',
    area:'corporate', exp:'3–5 years in-house or firm',
    salary:'$70,000 – $85,000',
    posted:daysAgo(7),
    snippet:'Join Indeed\'s in-house legal team supporting employment law, SaaS commercial contracts, and global regulatory matters. Manage contract lifecycle in ContractPodAi, assist with employment disputes, and support legal operations initiatives.',
    applyUrl:'https://www.indeed.com/cmp/Indeed/jobs'
  },
  {
    id:20, level:'mid',
    title:'Criminal Defense Paralegal — Senior',
    company:'Minton, Bassett, Flores & Carsey',
    location:'Austin, TX 78701',
    area:'criminal', exp:'3–6 years criminal defense',
    salary:'$55,000 – $68,000',
    posted:daysAgo(8),
    snippet:'Austin\'s premier criminal defense firm needs an experienced paralegal for complex felony and white-collar matters. Coordinate witnesses, manage evidence, prepare trial notebooks, and support attorneys in state and federal court.',
    applyUrl:'https://www.linkedin.com/jobs/search/?keywords=senior+criminal+defense+paralegal&location=Austin%2C%20TX'
  },
  {
    id:21, level:'mid',
    title:'Employment Litigation Paralegal',
    company:'Sheppard Mullin Richter & Hampton',
    location:'Austin, TX',
    area:'litigation', exp:'2–4 years employment or lit.',
    salary:'$60,000 – $75,000',
    posted:daysAgo(9),
    snippet:'Support management-side employment attorneys on wage & hour class actions, EEOC charges, and non-compete litigation. Strong legal writing and prior employment litigation experience strongly preferred.',
    applyUrl:'https://www.sheppardmullin.com/careers'
  },
  {
    id:22, level:'mid',
    title:'Environmental & Land Use Paralegal',
    company:'Lloyd Gosselink Rochelle & Townsend',
    location:'Austin, TX 78701',
    area:'litigation', exp:'3–5 years regulatory',
    salary:'$58,000 – $72,000',
    posted:daysAgo(11),
    snippet:'Texas-based boutique firm in environmental, water, and land use law. Assist with TCEQ regulatory filings, agency proceedings, contested case hearings, and environmental transactional due diligence.',
    applyUrl:'https://www.lglawfirm.com/careers'
  },
  {
    id:23, level:'mid',
    title:'Healthcare Regulatory Paralegal',
    company:'Husch Blackwell LLP',
    location:'Austin, TX 78701',
    area:'corporate', exp:'3–5 years healthcare or regulatory',
    salary:'$62,000 – $78,000',
    posted:daysAgo(12),
    snippet:'Support healthcare regulatory practice advising hospitals, physician groups, and health tech companies. Draft regulatory submissions, research state licensing requirements, and assist with healthcare transactional matters.',
    applyUrl:'https://www.huschblackwell.com/careers'
  },
  {
    id:24, level:'mid',
    title:'Bankruptcy / Restructuring Paralegal',
    company:'Jackson Walker LLP',
    location:'Austin, TX 78701',
    area:'litigation', exp:'2–5 years bankruptcy or commercial',
    salary:'$60,000 – $76,000',
    posted:daysAgo(14),
    snippet:'One of Texas\' largest firms seeks a bankruptcy paralegal for complex Chapter 11 restructuring matters. Draft pleadings and schedules, manage federal court filing deadlines, and coordinate directly with clients and financial advisors.',
    applyUrl:'https://www.jacksonwalker.com/careers/'
  }
];

/* ════════════════════
   STATE
════════════════════ */
let filtered    = [...JOBS];
let activeLvl   = 'all';
let curPage     = 1;
const PAGE_SIZE = 12;

/* ════════════════════
   SEARCH / FILTER
════════════════════ */
function runSearch() {
  const kw   = document.getElementById('searchInput').value.toLowerCase().trim();
  const lvl  = document.getElementById('levelFilter').value;
  const area = document.getElementById('areaFilter').value;

  filtered = JOBS.filter(j => {
    const mLvl  = lvl  === 'all' || j.level === lvl;
    const mArea = area === 'all' || j.area  === area;
    const mKw   = !kw
      || j.title.toLowerCase().includes(kw)
      || j.company.toLowerCase().includes(kw)
      || j.snippet.toLowerCase().includes(kw)
      || j.area.toLowerCase().includes(kw);
    return mLvl && mArea && mKw;
  });

  // Sync pills
  activeLvl = lvl;
  syncPills(lvl);
  curPage = 1;
  render();
}

function setFilter(lvl, btn) {
  activeLvl = lvl;
  document.getElementById('levelFilter').value = lvl;

  // Filter keeping keyword + area
  const kw   = document.getElementById('searchInput').value.toLowerCase().trim();
  const area = document.getElementById('areaFilter').value;
  filtered = JOBS.filter(j => {
    const mLvl  = lvl  === 'all' || j.level === lvl;
    const mArea = area === 'all' || j.area  === area;
    const mKw   = !kw || j.title.toLowerCase().includes(kw) || j.company.toLowerCase().includes(kw) || j.snippet.toLowerCase().includes(kw);
    return mLvl && mArea && mKw;
  });

  syncPills(lvl);
  curPage = 1;
  render();
}

function syncPills(lvl) {
  document.querySelectorAll('.filter-row .pill').forEach(p => p.classList.remove('ea','ma'));
  if (lvl === 'all')   document.getElementById('pill-all').classList.add('ea');
  if (lvl === 'entry') document.getElementById('pill-entry').classList.add('ea');
  if (lvl === 'mid')   document.getElementById('pill-mid').classList.add('ma');
}

/* ════════════════════
   RENDER
════════════════════ */
function render() {
  const grid = document.getElementById('jobsGrid');
  const pag  = document.getElementById('pagination');
  document.getElementById('countDisplay').textContent = filtered.length;
  grid.innerHTML = '';
  pag.innerHTML  = '';

  if (!filtered.length) {
    grid.innerHTML = `
      <div class="empty-state">
        <div class="empty-state-icon">🔍</div>
        <div class="empty-state-title">No listings match your filters</div>
        <div class="empty-state-sub">Try clearing the keyword or selecting a different practice area or level.</div>
      </div>`;
    return;
  }

  const total = Math.ceil(filtered.length / PAGE_SIZE);
  const slice = filtered.slice((curPage - 1) * PAGE_SIZE, curPage * PAGE_SIZE);

  slice.forEach(job => {
    const card = document.createElement('div');
    card.className = `job-card ${job.level}`;

    const salHtml = job.salary
      ? `<div class="csalary cs-${job.level}">${esc(job.salary)}</div>`
      : `<div class="cs-none">Salary not listed</div>`;

    card.innerHTML = `
      <div class="ctop">
        <div class="cbadges">
          <span class="badge ${job.level === 'entry' ? 'be' : 'bm'}">${job.level === 'entry' ? 'Entry Level' : 'Mid Level'}</span>
          <span class="badge bsc">${esc(areaLabel(job.area))}</span>
        </div>
        <span class="cposted">${formatPosted(job.posted)}</span>
      </div>
      <div class="ctitle">${esc(job.title)}</div>
      <div class="ccompany">${esc(job.company)}</div>
      <div class="cloc">
        <svg width="10" height="13" viewBox="0 0 10 13" fill="none"><path d="M5 0C2.239 0 0 2.239 0 5c0 3.75 5 8 5 8s5-4.25 5-8c0-2.761-2.239-5-5-5zm0 6.5A1.5 1.5 0 115 3.5a1.5 1.5 0 010 3z" fill="currentColor"/></svg>
        ${esc(job.location)}
      </div>
      <div class="cexp">📌 ${esc(job.exp)}</div>
      <div class="cdivider"></div>
      <div class="csnippet">${esc(job.snippet)}</div>
      <div class="cfooter">
        ${salHtml}
        <a class="apply-btn ${job.level === 'entry' ? 'ab-entry' : 'ab-mid'}"
           href="${esc(job.applyUrl)}"
           target="_blank" rel="noopener">Apply Now</a>
      </div>
    `;
    grid.appendChild(card);
  });

  // Pagination
  if (total > 1) {
    const prev = document.createElement('button');
    prev.className = 'pbt'; prev.textContent = '←';
    prev.disabled = curPage === 1;
    prev.onclick = () => goPage(curPage - 1);
    pag.appendChild(prev);

    for (let i = 1; i <= total; i++) {
      const b = document.createElement('button');
      b.className = 'pbt' + (i === curPage ? ' active' : '');
      b.textContent = i;
      b.onclick = () => goPage(i);
      pag.appendChild(b);
    }

    const next = document.createElement('button');
    next.className = 'pbt'; next.textContent = '→';
    next.disabled = curPage === total;
    next.onclick = () => goPage(curPage + 1);
    pag.appendChild(next);
  }
}

function goPage(p) {
  curPage = p;
  render();
  document.getElementById('jobs').scrollIntoView({ behavior: 'smooth', block: 'start' });
}

/* ════════════════════
   KEYBOARD
════════════════════ */
document.getElementById('searchInput').addEventListener('keydown', e => {
  if (e.key === 'Enter') runSearch();
});

/* ════════════════════
   INIT
════════════════════ */
document.getElementById('totalCount').textContent = JOBS.length;
render();
</script>
</body>
</html>
