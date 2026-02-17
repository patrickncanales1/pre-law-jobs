# pre-law-jobs

<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Austin Paralegal Jobs — Entry Level</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;1,400&family=DM+Mono:wght@300;400;500&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet" />
  <style>
    :root {
      --cream: #F5F0E8;
      --ink: #1A1612;
      --rust: #C45C2E;
      --gold: #C9963B;
      --muted: #7A7065;
      --card-bg: #FDFAF5;
      --border: #E0D8CC;
      --tag-bg: #EDE6D8;
    }

    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    html { scroll-behavior: smooth; }

    body {
      background-color: var(--cream);
      color: var(--ink);
      font-family: 'DM Sans', sans-serif;
      font-weight: 300;
      min-height: 100vh;
      overflow-x: hidden;
    }

    /* Grain overlay */
    body::before {
      content: '';
      position: fixed;
      inset: 0;
      background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='300' height='300'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='300' height='300' filter='url(%23n)' opacity='0.04'/%3E%3C/svg%3E");
      pointer-events: none;
      z-index: 1000;
      opacity: 0.6;
    }

    /* ── HEADER ─────────────────────────────── */
    header {
      border-bottom: 1px solid var(--border);
      padding: 2rem 4rem;
      display: flex;
      align-items: center;
      justify-content: space-between;
      position: sticky;
      top: 0;
      background: rgba(245, 240, 232, 0.92);
      backdrop-filter: blur(12px);
      z-index: 100;
    }

    .logo {
      display: flex;
      align-items: center;
      gap: 0.75rem;
    }

    .logo-mark {
      width: 36px;
      height: 36px;
      background: var(--rust);
      border-radius: 4px;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .logo-mark svg { fill: white; }

    .logo-text {
      font-family: 'DM Mono', monospace;
      font-size: 0.7rem;
      font-weight: 400;
      letter-spacing: 0.18em;
      text-transform: uppercase;
      color: var(--muted);
      line-height: 1.4;
    }

    .header-right {
      font-family: 'DM Mono', monospace;
      font-size: 0.68rem;
      color: var(--muted);
      letter-spacing: 0.1em;
      text-transform: uppercase;
    }

    /* ── HERO ─────────────────────────────── */
    .hero {
      padding: 5rem 4rem 4rem;
      max-width: 1200px;
      margin: 0 auto;
      display: grid;
      grid-template-columns: 1fr auto;
      gap: 2rem;
      align-items: end;
    }

    .hero-eyebrow {
      font-family: 'DM Mono', monospace;
      font-size: 0.68rem;
      letter-spacing: 0.2em;
      text-transform: uppercase;
      color: var(--rust);
      margin-bottom: 1.25rem;
      display: flex;
      align-items: center;
      gap: 0.75rem;
    }

    .hero-eyebrow::before {
      content: '';
      display: block;
      width: 24px;
      height: 1px;
      background: var(--rust);
    }

    h1 {
      font-family: 'Playfair Display', serif;
      font-size: clamp(2.8rem, 5vw, 4.5rem);
      font-weight: 700;
      line-height: 1.05;
      letter-spacing: -0.02em;
      color: var(--ink);
    }

    h1 em {
      font-style: italic;
      color: var(--rust);
    }

    .hero-sub {
      margin-top: 1.25rem;
      font-size: 1rem;
      color: var(--muted);
      font-weight: 300;
      max-width: 480px;
      line-height: 1.7;
    }

    .hero-stats {
      display: flex;
      flex-direction: column;
      align-items: flex-end;
      gap: 0.25rem;
    }

    .stat-num {
      font-family: 'Playfair Display', serif;
      font-size: 3.5rem;
      font-weight: 700;
      color: var(--ink);
      line-height: 1;
    }

    .stat-label {
      font-family: 'DM Mono', monospace;
      font-size: 0.65rem;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      color: var(--muted);
      text-align: right;
    }

    /* ── FILTERS ─────────────────────────────── */
    .filters-bar {
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 4rem 2.5rem;
      display: flex;
      align-items: center;
      gap: 1rem;
      flex-wrap: wrap;
    }

    .search-wrap {
      position: relative;
      flex: 1;
      min-width: 240px;
    }

    .search-wrap svg {
      position: absolute;
      left: 1rem;
      top: 50%;
      transform: translateY(-50%);
      color: var(--muted);
      pointer-events: none;
    }

    input[type="text"], select {
      font-family: 'DM Sans', sans-serif;
      font-size: 0.9rem;
      font-weight: 300;
      border: 1px solid var(--border);
      border-radius: 6px;
      background: var(--card-bg);
      color: var(--ink);
      transition: border-color 0.2s, box-shadow 0.2s;
      outline: none;
    }

    input[type="text"]:focus, select:focus {
      border-color: var(--rust);
      box-shadow: 0 0 0 3px rgba(196, 92, 46, 0.1);
    }

    #searchInput {
      width: 100%;
      padding: 0.75rem 1rem 0.75rem 2.8rem;
    }

    select {
      padding: 0.75rem 1rem;
      cursor: pointer;
      appearance: none;
      background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='12' height='12' viewBox='0 0 24 24' fill='none' stroke='%237A7065' stroke-width='2'%3E%3Cpolyline points='6,9 12,15 18,9'/%3E%3C/svg%3E");
      background-repeat: no-repeat;
      background-position: right 0.75rem center;
      padding-right: 2.25rem;
    }

    .btn {
      font-family: 'DM Mono', monospace;
      font-size: 0.72rem;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      padding: 0.75rem 1.5rem;
      border-radius: 6px;
      border: none;
      cursor: pointer;
      transition: all 0.2s;
      white-space: nowrap;
    }

    .btn-primary {
      background: var(--rust);
      color: white;
    }

    .btn-primary:hover {
      background: #b04e24;
      transform: translateY(-1px);
      box-shadow: 0 4px 16px rgba(196, 92, 46, 0.25);
    }

    .btn-ghost {
      background: transparent;
      color: var(--muted);
      border: 1px solid var(--border);
    }

    .btn-ghost:hover {
      border-color: var(--rust);
      color: var(--rust);
    }

    /* ── SETUP NOTICE ─────────────────────────────── */
    .setup-notice {
      max-width: 1200px;
      margin: 0 auto 2rem;
      padding: 0 4rem;
    }

    .notice-card {
      background: #FEF8EC;
      border: 1px solid #F0D898;
      border-radius: 10px;
      padding: 1.25rem 1.5rem;
      display: flex;
      align-items: flex-start;
      gap: 1rem;
    }

    .notice-icon {
      width: 20px;
      height: 20px;
      flex-shrink: 0;
      margin-top: 2px;
      color: var(--gold);
    }

    .notice-card h4 {
      font-family: 'DM Mono', monospace;
      font-size: 0.72rem;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      color: var(--gold);
      margin-bottom: 0.4rem;
    }

    .notice-card p {
      font-size: 0.87rem;
      color: #7A6830;
      line-height: 1.6;
    }

    .notice-card code {
      font-family: 'DM Mono', monospace;
      font-size: 0.8rem;
      background: rgba(201, 150, 59, 0.12);
      padding: 0.1em 0.35em;
      border-radius: 3px;
    }

    /* ── STATUS BAR ─────────────────────────────── */
    .status-bar {
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 4rem 1.5rem;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .results-count {
      font-family: 'DM Mono', monospace;
      font-size: 0.7rem;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      color: var(--muted);
    }

    .source-pills {
      display: flex;
      gap: 0.5rem;
    }

    .pill {
      font-family: 'DM Mono', monospace;
      font-size: 0.65rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      padding: 0.3rem 0.7rem;
      border-radius: 99px;
      background: var(--tag-bg);
      color: var(--muted);
    }

    .pill.adzuna { background: rgba(196, 92, 46, 0.1); color: var(--rust); }
    .pill.jooble { background: rgba(201, 150, 59, 0.1); color: var(--gold); }

    /* ── JOB GRID ─────────────────────────────── */
    #jobsContainer {
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 4rem 6rem;
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(340px, 1fr));
      gap: 1.25rem;
    }

    /* ── JOB CARD ─────────────────────────────── */
    .job-card {
      background: var(--card-bg);
      border: 1px solid var(--border);
      border-radius: 12px;
      padding: 1.5rem;
      display: flex;
      flex-direction: column;
      gap: 1rem;
      transition: transform 0.2s, box-shadow 0.2s, border-color 0.2s;
      animation: fadeUp 0.4s ease both;
      position: relative;
      overflow: hidden;
    }

    .job-card::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      height: 3px;
      background: linear-gradient(90deg, var(--rust), var(--gold));
      opacity: 0;
      transition: opacity 0.2s;
    }

    .job-card:hover {
      transform: translateY(-3px);
      box-shadow: 0 12px 40px rgba(26, 22, 18, 0.08);
      border-color: rgba(196, 92, 46, 0.3);
    }

    .job-card:hover::before { opacity: 1; }

    @keyframes fadeUp {
      from { opacity: 0; transform: translateY(16px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .card-header {
      display: flex;
      justify-content: space-between;
      align-items: flex-start;
      gap: 0.75rem;
    }

    .source-badge {
      font-family: 'DM Mono', monospace;
      font-size: 0.6rem;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      padding: 0.25rem 0.6rem;
      border-radius: 4px;
      flex-shrink: 0;
    }

    .source-adzuna {
      background: rgba(196, 92, 46, 0.1);
      color: var(--rust);
    }

    .source-jooble {
      background: rgba(201, 150, 59, 0.1);
      color: var(--gold);
    }

    .source-other {
      background: var(--tag-bg);
      color: var(--muted);
    }

    .job-title {
      font-family: 'Playfair Display', serif;
      font-size: 1.15rem;
      font-weight: 700;
      line-height: 1.3;
      color: var(--ink);
      text-decoration: none;
      transition: color 0.2s;
    }

    .job-title:hover { color: var(--rust); }

    .company-row {
      display: flex;
      align-items: center;
      gap: 0.5rem;
    }

    .company-icon {
      width: 32px;
      height: 32px;
      border-radius: 6px;
      background: var(--tag-bg);
      display: flex;
      align-items: center;
      justify-content: center;
      font-family: 'Playfair Display', serif;
      font-size: 0.85rem;
      font-weight: 700;
      color: var(--muted);
      flex-shrink: 0;
    }

    .company-info { flex: 1; min-width: 0; }

    .company-name {
      font-size: 0.88rem;
      font-weight: 500;
      color: var(--ink);
      white-space: nowrap;
      overflow: hidden;
      text-overflow: ellipsis;
    }

    .job-location {
      font-size: 0.78rem;
      color: var(--muted);
      display: flex;
      align-items: center;
      gap: 0.3rem;
    }

    .job-snippet {
      font-size: 0.85rem;
      color: var(--muted);
      line-height: 1.65;
      display: -webkit-box;
      -webkit-line-clamp: 3;
      -webkit-box-orient: vertical;
      overflow: hidden;
    }

    .card-footer {
      display: flex;
      align-items: center;
      justify-content: space-between;
      margin-top: auto;
      padding-top: 0.75rem;
      border-top: 1px solid var(--border);
    }

    .salary-tag {
      font-family: 'DM Mono', monospace;
      font-size: 0.72rem;
      color: var(--rust);
      font-weight: 500;
    }

    .date-tag {
      font-family: 'DM Mono', monospace;
      font-size: 0.65rem;
      color: var(--muted);
      letter-spacing: 0.05em;
    }

    .apply-btn {
      font-family: 'DM Mono', monospace;
      font-size: 0.68rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      text-decoration: none;
      color: var(--rust);
      padding: 0.4rem 0.85rem;
      border: 1px solid rgba(196, 92, 46, 0.35);
      border-radius: 4px;
      transition: all 0.2s;
    }

    .apply-btn:hover {
      background: var(--rust);
      color: white;
      border-color: var(--rust);
    }

    /* ── LOADING STATE ─────────────────────────────── */
    #loadingState {
      max-width: 1200px;
      margin: 0 auto;
      padding: 4rem;
      display: none;
      flex-direction: column;
      align-items: center;
      gap: 1.25rem;
    }

    .spinner {
      width: 40px;
      height: 40px;
      border: 2px solid var(--border);
      border-top-color: var(--rust);
      border-radius: 50%;
      animation: spin 0.8s linear infinite;
    }

    @keyframes spin { to { transform: rotate(360deg); } }

    .loading-text {
      font-family: 'DM Mono', monospace;
      font-size: 0.7rem;
      letter-spacing: 0.18em;
      text-transform: uppercase;
      color: var(--muted);
    }

    /* ── EMPTY STATE ─────────────────────────────── */
    #emptyState {
      max-width: 1200px;
      margin: 0 auto;
      padding: 4rem;
      text-align: center;
      display: none;
    }

    .empty-icon {
      font-size: 3rem;
      margin-bottom: 1rem;
    }

    .empty-title {
      font-family: 'Playfair Display', serif;
      font-size: 1.5rem;
      margin-bottom: 0.5rem;
    }

    .empty-sub {
      font-size: 0.9rem;
      color: var(--muted);
    }

    /* ── DEMO DATA BANNER ─────────────────────────────── */
    .demo-banner {
      max-width: 1200px;
      margin: 0 auto 1.5rem;
      padding: 0 4rem;
    }

    .demo-strip {
      background: rgba(196, 92, 46, 0.07);
      border: 1px dashed rgba(196, 92, 46, 0.3);
      border-radius: 6px;
      padding: 0.6rem 1rem;
      font-family: 'DM Mono', monospace;
      font-size: 0.68rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      color: var(--rust);
      text-align: center;
    }

    /* ── INSTRUCTIONS PANEL ─────────────────────────────── */
    .instructions {
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 4rem 3rem;
    }

    details {
      border: 1px solid var(--border);
      border-radius: 10px;
      overflow: hidden;
    }

    summary {
      padding: 1.25rem 1.5rem;
      font-family: 'DM Mono', monospace;
      font-size: 0.75rem;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      cursor: pointer;
      display: flex;
      align-items: center;
      justify-content: space-between;
      background: var(--card-bg);
      color: var(--muted);
      list-style: none;
      user-select: none;
    }

    summary:hover { color: var(--ink); }
    summary::after { content: '+'; font-size: 1.2rem; }
    details[open] summary::after { content: '−'; }

    .instructions-body {
      padding: 1.5rem;
      background: var(--card-bg);
      border-top: 1px solid var(--border);
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 2rem;
    }

    .instr-col h3 {
      font-family: 'DM Mono', monospace;
      font-size: 0.7rem;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      color: var(--rust);
      margin-bottom: 1rem;
    }

    .step {
      display: flex;
      gap: 1rem;
      margin-bottom: 1rem;
      align-items: flex-start;
    }

    .step-num {
      width: 24px;
      height: 24px;
      border-radius: 50%;
      background: var(--ink);
      color: var(--cream);
      font-family: 'DM Mono', monospace;
      font-size: 0.7rem;
      display: flex;
      align-items: center;
      justify-content: center;
      flex-shrink: 0;
    }

    .step-text {
      font-size: 0.85rem;
      color: var(--muted);
      line-height: 1.6;
    }

    .step-text code {
      font-family: 'DM Mono', monospace;
      font-size: 0.78rem;
      background: var(--tag-bg);
      padding: 0.1em 0.35em;
      border-radius: 3px;
      color: var(--ink);
    }

    .code-block {
      background: var(--ink);
      color: #E8DFD0;
      border-radius: 8px;
      padding: 1rem 1.25rem;
      font-family: 'DM Mono', monospace;
      font-size: 0.78rem;
      line-height: 1.7;
      overflow-x: auto;
      margin-top: 0.5rem;
    }

    .code-block .kw { color: #C45C2E; }
    .code-block .str { color: #C9963B; }
    .code-block .cmt { color: #7A7065; }

    /* ── FOOTER ─────────────────────────────── */
    footer {
      border-top: 1px solid var(--border);
      padding: 2rem 4rem;
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1200px;
      margin: 0 auto;
    }

    .footer-copy {
      font-family: 'DM Mono', monospace;
      font-size: 0.65rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      color: var(--muted);
    }

    .footer-links {
      display: flex;
      gap: 1.5rem;
    }

    .footer-links a {
      font-family: 'DM Mono', monospace;
      font-size: 0.65rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      color: var(--muted);
      text-decoration: none;
      transition: color 0.2s;
    }

    .footer-links a:hover { color: var(--rust); }

    /* ── RESPONSIVE ─────────────────────────────── */
    @media (max-width: 768px) {
      header { padding: 1.25rem 1.5rem; }
      .hero { padding: 3rem 1.5rem 2rem; grid-template-columns: 1fr; }
      .hero-stats { align-items: flex-start; }
      .filters-bar { padding: 0 1.5rem 2rem; }
      .setup-notice, .demo-banner, .instructions { padding-left: 1.5rem; padding-right: 1.5rem; }
      #jobsContainer { padding: 0 1.5rem 4rem; grid-template-columns: 1fr; }
      .status-bar { padding: 0 1.5rem 1.5rem; flex-direction: column; align-items: flex-start; gap: 0.75rem; }
      .instructions-body { grid-template-columns: 1fr; }
      footer { padding: 1.5rem; flex-direction: column; gap: 1rem; }
    }
  </style>
</head>
<body>

  <!-- ─── HEADER ──────────────────────────────────────── -->
  <header>
    <div class="logo">
      <div class="logo-mark">
        <svg width="18" height="18" viewBox="0 0 24 24">
          <path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/>
          <polyline points="14 2 14 8 20 8" fill="none" stroke="white" stroke-width="1.5"/>
          <line x1="16" y1="13" x2="8" y2="13" fill="none" stroke="white" stroke-width="1.5"/>
          <line x1="16" y1="17" x2="8" y2="17" fill="none" stroke="white" stroke-width="1.5"/>
          <polyline points="10 9 9 9 8 9" fill="none" stroke="white" stroke-width="1.5"/>
        </svg>
      </div>
      <div class="logo-text">
        Austin Legal<br/>Career Board
      </div>
    </div>
    <div class="header-right">Austin, TX · Entry Level</div>
  </header>

  <!-- ─── HERO ──────────────────────────────────────── -->
  <section class="hero">
    <div>
      <div class="hero-eyebrow">Live job aggregator</div>
      <h1>Find Your Place<br/>in Austin <em>Law.</em></h1>
      <p class="hero-sub">Curated entry-level paralegal openings across Austin-area law firms and corporate legal departments — aggregated live from Adzuna &amp; Jooble.</p>
    </div>
    <div class="hero-stats">
      <div class="stat-num" id="heroCount">—</div>
      <div class="stat-label">Listings<br/>Loaded</div>
    </div>
  </section>

  <!-- ─── FILTERS ──────────────────────────────────────── -->
  <div class="filters-bar">
    <div class="search-wrap">
      <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
        <circle cx="11" cy="11" r="8"/><line x1="21" y1="21" x2="16.65" y2="16.65"/>
      </svg>
      <input type="text" id="searchInput" placeholder="Search title, company, keyword…" />
    </div>
    <select id="sourceFilter">
      <option value="all">All Sources</option>
      <option value="Adzuna">Adzuna</option>
      <option value="Jooble">Jooble</option>
    </select>
    <select id="sortFilter">
      <option value="date">Newest First</option>
      <option value="title">A → Z</option>
      <option value="company">By Company</option>
    </select>
    <button class="btn btn-primary" onclick="loadJobs()">Refresh</button>
    <button class="btn btn-ghost" onclick="clearFilters()">Clear</button>
  </div>

  <!-- ─── SETUP NOTICE ──────────────────────────────────────── -->
  <div class="setup-notice">
    <div class="notice-card">
      <svg class="notice-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
        <circle cx="12" cy="12" r="10"/><line x1="12" y1="8" x2="12" y2="12"/><line x1="12" y1="16" x2="12.01" y2="16"/>
      </svg>
      <div>
        <h4>Developer Setup Required</h4>
        <p>This page fetches live data from your backend. Set <code>BACKEND_URL</code> at the top of the script to your Netlify / Vercel / Cloudflare Workers endpoint (e.g. <code>https://your-site.netlify.app/api/jobs</code>). Until then, sample listings are shown below. See the setup guide for full instructions.</p>
      </div>
    </div>
  </div>

  <!-- ─── DEMO BANNER ──────────────────────────────────────── -->
  <div class="demo-banner" id="demoBanner">
    <div class="demo-strip">⚡ Showing sample data · Connect your backend to load live listings</div>
  </div>

  <!-- ─── STATUS BAR ──────────────────────────────────────── -->
  <div class="status-bar">
    <div class="results-count" id="resultsCount">— listings found</div>
    <div class="source-pills">
      <span class="pill adzuna">Adzuna</span>
      <span class="pill jooble">Jooble</span>
      <span class="pill">Live Feed</span>
    </div>
  </div>

  <!-- ─── LOADING ──────────────────────────────────────── -->
  <div id="loadingState">
    <div class="spinner"></div>
    <div class="loading-text">Fetching listings…</div>
  </div>

  <!-- ─── EMPTY STATE ──────────────────────────────────────── -->
  <div id="emptyState">
    <div class="empty-icon">📂</div>
    <div class="empty-title">No listings match</div>
    <div class="empty-sub">Try adjusting your search or clearing filters.</div>
  </div>

  <!-- ─── JOB CARDS ──────────────────────────────────────── -->
  <div id="jobsContainer"></div>

  <!-- ─── SETUP INSTRUCTIONS ──────────────────────────────────────── -->
  <div class="instructions">
    <details>
      <summary>Developer Setup Guide — Connect Live Data</summary>
      <div class="instructions-body">
        <div class="instr-col">
          <h3>Step-by-step</h3>
          <div class="step">
            <div class="step-num">1</div>
            <div class="step-text">Register for an <strong>Adzuna</strong> developer account at <code>developer.adzuna.com</code> to get your <code>app_id</code> and <code>app_key</code>.</div>
          </div>
          <div class="step">
            <div class="step-num">2</div>
            <div class="step-text">Register for a <strong>Jooble</strong> API key at <code>help.jooble.org</code> and note your key for the POST endpoint.</div>
          </div>
          <div class="step">
            <div class="step-num">3</div>
            <div class="step-text">Deploy the Node.js aggregation server (see right) to <strong>Netlify Functions</strong>, <strong>Vercel</strong>, or <strong>Cloudflare Workers</strong>. Set API keys as environment variables — never hardcode them.</div>
          </div>
          <div class="step">
            <div class="step-num">4</div>
            <div class="step-text">Update the <code>BACKEND_URL</code> constant at the top of this page's <code>&lt;script&gt;</code> to your deployed endpoint URL.</div>
          </div>
          <div class="step">
            <div class="step-num">5</div>
            <div class="step-text">Push this <code>index.html</code> to your GitHub repo. Enable <strong>GitHub Pages</strong> from Settings → Pages → Deploy from branch.</div>
          </div>
        </div>
        <div class="instr-col">
          <h3>Backend endpoint (Node.js)</h3>
          <div class="code-block">
<span class="cmt">// Netlify Function: netlify/functions/jobs.js</span>
<span class="kw">const</span> fetch = <span class="kw">require</span>(<span class="str">'node-fetch'</span>);

exports.handler = <span class="kw">async</span> (event) => {
  <span class="kw">const</span> q = event.queryStringParameters;
  <span class="kw">const</span> query = q?.query || <span class="str">'paralegal'</span>;
  <span class="kw">const</span> loc   = q?.location || <span class="str">'Austin, TX'</span>;

  <span class="cmt">// Fetch Adzuna</span>
  <span class="kw">const</span> azUrl = <span class="kw">new</span> URL(
    <span class="str">'https://api.adzuna.com/v1/api/jobs/us/search/1'</span>);
  azUrl.searchParams.set(<span class="str">'app_id'</span>, process.env.ADZUNA_APP_ID);
  azUrl.searchParams.set(<span class="str">'app_key'</span>, process.env.ADZUNA_APP_KEY);
  azUrl.searchParams.set(<span class="str">'what'</span>, query);
  azUrl.searchParams.set(<span class="str">'where'</span>, loc);
  <span class="kw">const</span> az = <span class="kw">await</span> fetch(azUrl).then(r => r.json());

  <span class="cmt">// Fetch Jooble</span>
  <span class="kw">const</span> jb = <span class="kw">await</span> fetch(
    <span class="str">`https://jooble.org/api/${process.env.JOOBLE_KEY}`</span>,
    { method: <span class="str">'POST'</span>,
      headers: {<span class="str">'Content-Type'</span>:<span class="str">'application/json'</span>},
      body: JSON.stringify({ keywords: query, location: loc })
    }).then(r => r.json());

  <span class="cmt">// Normalize + de-dup + return</span>
  <span class="kw">const</span> jobs = [...normalize(az), ...normalize(jb)];
  <span class="kw">return</span> { statusCode: 200,
    headers: {<span class="str">'Access-Control-Allow-Origin'</span>: <span class="str">'*'</span>},
    body: JSON.stringify({ jobs }) };
};
          </div>
        </div>
      </div>
    </details>
  </div>

  <!-- ─── FOOTER ──────────────────────────────────────── -->
  <footer>
    <div class="footer-copy">Austin Legal Career Board · Powered by Adzuna &amp; Jooble</div>
    <div class="footer-links">
      <a href="https://developer.adzuna.com" target="_blank" rel="noopener">Adzuna API</a>
      <a href="https://help.jooble.org/en/support/solutions/articles/60001448238" target="_blank" rel="noopener">Jooble API</a>
      <a href="https://pages.github.com" target="_blank" rel="noopener">GitHub Pages</a>
    </div>
  </footer>

  <!-- ─── SCRIPT ──────────────────────────────────────── -->
  <script>
    // ─────────────────────────────────────────────────────────
    // 🔧 CONFIGURE THIS: Replace with your deployed backend URL
    //    e.g. 'https://your-site.netlify.app/api/jobs'
    //         or '/.netlify/functions/jobs'
    const BACKEND_URL = '';
    // ─────────────────────────────────────────────────────────

    const SAMPLE_JOBS = [
      { source: 'Adzuna', title: 'Entry-Level Paralegal', company: 'Martin & Hollis LLP', location: 'Austin, TX', salary: '$38,000 - $48,000', snippet: 'Assist senior attorneys with legal research, document preparation, and case management for a fast-growing civil litigation firm in downtown Austin. No experience required — training provided.', link: '#', posted: '2025-02-14' },
      { source: 'Jooble', title: 'Legal Assistant / Paralegal I', company: 'Lone Star Corporate Legal', location: 'Austin, TX', salary: '$40,000 - $52,000', snippet: 'Support in-house legal team with contract review, compliance documentation, and administrative tasks. Ideal for recent graduates with a paralegal certificate or political science degree.', link: '#', posted: '2025-02-13' },
      { source: 'Adzuna', title: 'Paralegal — Family Law', company: 'Hayes Family Law Group', location: 'Round Rock, TX', salary: '$36,000 - $44,000', snippet: 'Assist attorneys in drafting pleadings, organizing case files, client correspondence, and scheduling hearings. Bilingual (English/Spanish) a strong plus for our diverse client base.', link: '#', posted: '2025-02-12' },
      { source: 'Jooble', title: 'Junior Paralegal — Real Estate', company: 'Texas Title & Realty Law', location: 'Austin, TX', salary: null, snippet: 'Join our real estate transactions team. Duties include title searches, lien releases, closing document preparation, and coordination with escrow and title companies across Central Texas.', link: '#', posted: '2025-02-11' },
      { source: 'Adzuna', title: 'Litigation Paralegal (Entry Level)', company: 'Barrera, Reyes & Okafor', location: 'Austin, TX', salary: '$42,000 - $55,000', snippet: 'Support a busy litigation team with discovery management, deposition scheduling, exhibit preparation, and file maintenance. Strong organizational skills and proficiency with Microsoft Office required.', link: '#', posted: '2025-02-10' },
      { source: 'Jooble', title: 'Legal Operations Coordinator', company: 'Dell Technologies — Legal Dept.', location: 'Austin, TX (Hybrid)', salary: '$48,000 - $58,000', snippet: 'Assist in-house counsel with vendor contracts, NDA management, and IP tracking dashboards. This is a great opportunity to join a Fortune 500 legal team at an early career stage.', link: '#', posted: '2025-02-09' },
    ];

    let allJobs = [];

    async function loadJobs() {
      const container = document.getElementById('jobsContainer');
      const loading = document.getElementById('loadingState');
      const emptyState = document.getElementById('emptyState');
      const demoBanner = document.getElementById('demoBanner');

      container.innerHTML = '';
      loading.style.display = 'flex';
      emptyState.style.display = 'none';

      if (!BACKEND_URL) {
        await new Promise(r => setTimeout(r, 600));
        allJobs = SAMPLE_JOBS;
        demoBanner.style.display = 'block';
      } else {
        demoBanner.style.display = 'none';
        try {
          const res = await fetch(
            `${BACKEND_URL}?query=entry+level+paralegal&location=Austin,+TX`
          );
          const data = await res.json();
          allJobs = data.jobs || [];
        } catch (err) {
          console.error('Failed to fetch jobs:', err);
          allJobs = SAMPLE_JOBS;
          demoBanner.style.display = 'block';
        }
      }

      loading.style.display = 'none';
      applyFilters();
    }

    function applyFilters() {
      const query  = document.getElementById('searchInput').value.toLowerCase();
      const source = document.getElementById('sourceFilter').value;
      const sort   = document.getElementById('sortFilter').value;

      let filtered = allJobs.filter(j => {
        const matchSearch = !query || [j.title, j.company, j.snippet, j.location]
          .some(f => f && f.toLowerCase().includes(query));
        const matchSource = source === 'all' || (j.source || '').toLowerCase().includes(source.toLowerCase());
        return matchSearch && matchSource;
      });

      if (sort === 'date') {
        filtered.sort((a, b) => new Date(b.posted || 0) - new Date(a.posted || 0));
      } else if (sort === 'title') {
        filtered.sort((a, b) => (a.title || '').localeCompare(b.title || ''));
      } else if (sort === 'company') {
        filtered.sort((a, b) => (a.company || '').localeCompare(b.company || ''));
      }

      renderJobs(filtered);
    }

    function renderJobs(jobs) {
      const container = document.getElementById('jobsContainer');
      const emptyState = document.getElementById('emptyState');
      const count = document.getElementById('resultsCount');
      const heroCount = document.getElementById('heroCount');

      container.innerHTML = '';
      count.textContent = `${jobs.length} listing${jobs.length !== 1 ? 's' : ''} found`;
      heroCount.textContent = jobs.length;

      if (jobs.length === 0) {
        emptyState.style.display = 'block';
        return;
      }

      emptyState.style.display = 'none';
      jobs.forEach((job, i) => {
        const card = buildCard(job, i);
        container.appendChild(card);
      });
    }

    function buildCard(job, index) {
      const div = document.createElement('div');
      div.className = 'job-card';
      div.style.animationDelay = `${index * 50}ms`;

      const sourceClass = job.source === 'Adzuna' ? 'source-adzuna'
                        : job.source === 'Jooble' ? 'source-jooble'
                        : 'source-other';

      const initial = (job.company || '?')[0].toUpperCase();
      const dateStr = job.posted ? formatDate(job.posted) : 'Recently posted';
      const snippet = job.snippet ? job.snippet.slice(0, 220) + (job.snippet.length > 220 ? '…' : '') : '';

      div.innerHTML = `
        <div class="card-header">
          <a class="job-title" href="${job.link || '#'}" target="_blank" rel="noopener">
            ${escHtml(job.title || 'Paralegal Position')}
          </a>
          <span class="source-badge ${sourceClass}">${escHtml(job.source || 'Other')}</span>
        </div>
        <div class="company-row">
          <div class="company-icon">${initial}</div>
          <div class="company-info">
            <div class="company-name">${escHtml(job.company || 'Company Not Listed')}</div>
            <div class="job-location">
              <svg width="11" height="11" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5">
                <path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"/>
                <circle cx="12" cy="10" r="3"/>
              </svg>
              ${escHtml(job.location || 'Austin, TX')}
            </div>
          </div>
        </div>
        ${snippet ? `<p class="job-snippet">${escHtml(snippet)}</p>` : ''}
        <div class="card-footer">
          <div>
            ${job.salary ? `<div class="salary-tag">💵 ${escHtml(job.salary)}</div>` : ''}
            <div class="date-tag">${dateStr}</div>
          </div>
          <a class="apply-btn" href="${job.link || '#'}" target="_blank" rel="noopener">Apply →</a>
        </div>
      `;
      return div;
    }

    function formatDate(dateStr) {
      try {
        const d = new Date(dateStr);
        return d.toLocaleDateString('en-US', { month: 'short', day: 'numeric', year: 'numeric' });
      } catch { return dateStr; }
    }

    function escHtml(str) {
      return String(str)
        .replace(/&/g, '&amp;')
        .replace(/</g, '&lt;')
        .replace(/>/g, '&gt;')
        .replace(/"/g, '&quot;');
    }

    function clearFilters() {
      document.getElementById('searchInput').value = '';
      document.getElementById('sourceFilter').value = 'all';
      document.getElementById('sortFilter').value = 'date';
      applyFilters();
    }

    // Live filter on input
    document.getElementById('searchInput').addEventListener('input', applyFilters);
    document.getElementById('sourceFilter').addEventListener('change', applyFilters);
    document.getElementById('sortFilter').addEventListener('change', applyFilters);

    // Load on page ready
    loadJobs();
  </script>

</body>
</html>
