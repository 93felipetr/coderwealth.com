---
layout: default
title: Coder Wealth
---

<div class="container">
  <header class="header">
    <div class="logo">
      <span class="logo-icon">⚡</span>
      <span class="logo-text">CODERWEALTH</span>
    </div>
    <nav class="nav">
      <a href="#tech">Tech</a>
      <a href="#investing">Investing</a>
      <a href="#education">Education</a>
      <a href="#tools">Tools</a>
    </nav>
  </header>

  <section class="hero">
    <h1 class="hero-title">Master DevOps & Financial Independence</h1>
    <p class="hero-desc">Your definitive resource for building wealth through technology. High-level tutorials, proven investment strategies, and productivity tools for developers.</p>
    <a href="#articles" class="btn">Explore Articles</a>
  </section>

  <div class="grid-layout">
    <section id="articles" class="left-col">
      <h2 class="section-title">Latest Articles</h2>
      <div class="article-list">

        <article class="article-card">
          <div class="article-meta">
            <span class="badge cat-invest">Investing</span>
            <span class="date">Jan 27, 2026</span>
          </div>
          <div class="article-content">
            <h3 class="article-title"><a href="/2026/01/27/fire-strategy-tech-workers-2026/">FIRE Strategy for Tech Workers: Complete 2026 Guide</a></h3>
            <p class="excerpt">Achieve financial independence and retire early using your high developer salary and passive income streams.</p>
          </div>
          <div class="article-footer">
            <span class="read-more">Read Article &rarr;</span>
          </div>
        </article>

        <article class="article-card">
          <div class="article-meta">
            <span class="badge cat-invest">Investing</span>
            <span class="date">Jan 27, 2026</span>
          </div>
          <div class="article-content">
            <h3 class="article-title"><a href="/2026/01/27/realestate-investing-tech-workers-2026/">Real Estate Investing for Tech Workers: Complete 2026 Guide</a></h3>
            <p class="excerpt">Build passive income through REITs, crowdfunding, turnkey rentals, and international properties.</p>
          </div>
          <div class="article-footer">
            <span class="read-more">Read Article &rarr;</span>
          </div>
        </article>

        <article class="article-card">
          <div class="article-meta">
            <span class="badge cat-invest">Investing</span>
            <span class="date">Jan 27, 2026</span>
          </div>
          <div class="article-content">
            <h3 class="article-title"><a href="/2026/01/27/crypto-defi-strategies-2026/">Crypto & DeFi Strategies for 2026: Complete Guide</a></h3>
            <p class="excerpt">Master blockchain investing, staking (5-14% APY), yield farming, and secure Web3 protocols.</p>
          </div>
          <div class="article-footer">
            <span class="read-more">Read Article &rarr;</span>
          </div>
        </article>

        <article class="article-card">
          <div class="article-meta">
            <span class="badge cat-tech">Technology</span>
            <span class="date">Jan 27, 2026</span>
          </div>
          <div class="article-content">
            <h3 class="article-title"><a href="/2026/01/27/terraform-iac-complete-guide-2026/">Complete Terraform Guide: Infrastructure as Code (IaC) for 2026</a></h3>
            <p class="excerpt">Automate AWS, Azure, and GCP infrastructure. Master state management, modules, and CI/CD integration.</p>
          </div>
          <div class="article-footer">
            <span class="read-more">Read Article &rarr;</span>
          </div>
        </article>

      </div>
    </section>

    <section class="right-col">
      <h2 class="section-title">Categories</h2>
      <div class="category-list">

        <div class="category-card">
          <span class="cat-icon">⚡</span>
          <h4 class="cat-title">Technology</h4>
          <p class="cat-desc">Cloud, DevOps, Automation, Security, and Architecture.</p>
          <a href="#tech" class="cat-link">Explore Tech</a>
        </div>

        <div class="category-card">
          <span class="cat-icon">💰</span>
          <h4 class="cat-title">Investing</h4>
          <p class="cat-desc">Stocks, ETFs, FIRE, Real Estate, Crypto, and DeFi.</p>
          <a href="#investing" class="cat-link">Explore Investing</a>
        </div>

        <div class="category-card">
          <span class="cat-icon">🎓</span>
          <h4 class="cat-title">Education</h4>
          <p class="cat-desc">Certifications, Study Guides, Tutorials, and System Design.</p>
          <a href="#education" class="cat-link">Explore Education</a>
        </div>

        <div class="category-card">
          <span class="cat-icon">🛠️</span>
          <h4 class="cat-title">Tools</h4>
          <p class="cat-desc">Productivity, CRM, Developer Tools, and API Management.</p>
          <a href="#tools" class="cat-link">Explore Tools</a>
        </div>

      </div>
    </section>
  </div>

  <footer class="footer">
    <p>&copy; 2026 Coder Wealth. Build wealth through code and investing.</p>
    <div class="footer-nav">
      <a href="https://twitter.com/coderwealth">Twitter</a>
      <a href="https://github.com/93felipetr/coderwealth">GitHub</a>
    </div>
  </footer>

</div>

<style>
  /* CORE VARIABLES */
  :root {
    --primary: #0ea5e9;
    --primary-dark: #0c4a6e;
    --accent: #0d6efd;
    --bg-body: #f8f9fa;
    --bg-card: #ffffff;
    --text-main: #212529;
    --text-muted: #6c757d;
    --border: #e9ecef;
    --shadow: 0 4px 6px rgba(0,0,0,0.1);
    --radius: 0.5rem;
    --font-sans: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
  }

  /* RESET */
  * { box-sizing: border-box; margin: 0; padding: 0; }

  body {
    font-family: var(--font-sans);
    background-color: var(--bg-body);
    color: var(--text-main);
    line-height: 1.6;
    -webkit-font-smoothing: antialiased;
  }

  a { color: var(--primary); text-decoration: none; transition: color 0.2s ease; }
  a:hover { color: var(--primary-dark); }

  .container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 1rem;
  }

  /* HEADER */
  .header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1.5rem 1rem;
    background: var(--bg-card);
    border-bottom: 1px solid var(--border);
    box-shadow: var(--shadow);
  }
  .logo { display: flex; align-items: center; gap: 0.75rem; }
  .logo-icon { font-size: 1.5rem; }
  .logo-text {
    font-size: 1.5rem;
    font-weight: 800;
    letter-spacing: 1px;
    text-transform: uppercase;
    background: linear-gradient(135deg, var(--primary), var(--accent));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    color: transparent;
  }
  .nav { display: flex; gap: 1.5rem; }
  .nav a {
    font-size: 1rem;
    font-weight: 600;
    text-transform: uppercase;
    letter-spacing: 0.05em;
    color: var(--text-muted);
  }
  .nav a:hover { color: var(--primary); }

  /* HERO */
  .hero {
    text-align: center;
    padding: 4rem 1rem;
    background: linear-gradient(135deg, var(--bg-card) 0%, #f0f9ff 100%);
    border-bottom: 1px solid var(--border);
    margin-bottom: 2rem;
  }
  .hero-title { font-size: 2.5rem; font-weight: 800; margin-bottom: 1rem; color: var(--text-main); }
  .hero-desc { font-size: 1.25rem; color: var(--text-muted); max-width: 700px; margin: 0 auto; }
  .btn {
    display: inline-block;
    background: var(--primary);
    color: white;
    padding: 1rem 2rem;
    border-radius: var(--radius);
    font-weight: 700;
    font-size: 1.1rem;
    transition: transform 0.2s ease, box-shadow 0.2s ease;
  }
  .btn:hover { transform: translateY(-2px); box-shadow: 0 6px 12px rgba(14, 165, 233, 0.2); }

  /* GRID LAYOUT */
  .grid-layout { display: grid; grid-template-columns: 2fr 1fr; gap: 2rem; margin-bottom: 2rem; }
  @media (max-width: 900px) { .grid-layout { grid-template-columns: 1fr; } }

  .left-col, .right-col { display: flex; flex-direction: column; }

  /* SECTION TITLE */
  .section-title {
    font-size: 1.5rem;
    font-weight: 700;
    color: var(--text-main);
    margin-bottom: 1.5rem;
    padding-bottom: 0.5rem;
    border-bottom: 3px solid var(--primary);
  }

  /* ARTICLE LIST */
  .article-list { display: flex; flex-direction: column; gap: 1.5rem; }
  .article-card {
    background: var(--bg-card);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    padding: 1.5rem;
    transition: transform 0.2s ease, box-shadow 0.2s ease;
  }
  .article-card:hover {
    transform: translateY(-4px);
    box-shadow: 0 12px 20px rgba(14, 165, 233, 0.15);
    border-color: var(--primary);
  }
  .article-meta { display: flex; justify-content: space-between; margin-bottom: 1rem; padding-bottom: 1rem; border-bottom: 1px dashed var(--border); }
  .badge {
    font-size: 0.8rem;
    font-weight: 700;
    padding: 0.25rem 0.75rem;
    border-radius: 9999px;
    text-transform: uppercase;
    letter-spacing: 0.05em;
  }
  .cat-invest { background: #e3f2fd; color: #1c3ed1; }
  .cat-tech { background: #d1e7dd; color: #0f172a; }
  .date { font-size: 0.9rem; color: var(--text-muted); font-style: italic; }
  .article-title { margin: 0 0 1rem 0; font-size: 1.35rem; font-weight: 700; line-height: 1.3; }
  .article-title a { color: var(--text-main); display: block; }
  .article-title a:hover { color: var(--primary); }
  .excerpt { font-size: 1rem; color: var(--text-muted); margin-bottom: 1.5rem; line-height: 1.5; }
  .article-footer { display: flex; justify-content: flex-end; align-items: center; margin-top: auto; padding-top: 1rem; border-top: 1px solid var(--border); }
  .read-more {
    font-size: 0.9rem;
    font-weight: 600;
    text-transform: uppercase;
    letter-spacing: 0.05em;
    color: var(--primary);
  }
  .read-more::after { content: '→'; margin-left: 0.5rem; }

  /* CATEGORY LIST */
  .category-list { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 1rem; }
  .category-card {
    background: var(--bg-card);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    padding: 2rem 1rem;
    text-align: center;
    transition: transform 0.2s ease, box-shadow 0.2s ease;
  }
  .category-card:hover {
    transform: translateY(-4px);
    box-shadow: 0 12px 20px rgba(14, 165, 233, 0.15);
    border-color: var(--primary);
  }
  .cat-icon { font-size: 2.5rem; margin-bottom: 1rem; display: block; }
  .cat-title { font-size: 1.25rem; font-weight: 700; margin-bottom: 0.5rem; color: var(--text-main); }
  .cat-desc { font-size: 1rem; color: var(--text-muted); line-height: 1.5; margin-bottom: 1.5rem; }
  .cat-link {
    display: inline-block;
    margin-top: 1.5rem;
    padding: 0.75rem 1.5rem;
    background: var(--bg-body);
    color: var(--primary);
    border-radius: 9999px;
    font-weight: 600;
    text-transform: uppercase;
    letter-spacing: 0.05em;
    border: 1px solid var(--border);
    transition: all 0.2s ease;
  }
  .cat-link:hover {
    background: var(--primary);
    color: white;
    border-color: var(--primary);
  }

  /* FOOTER */
  .footer {
    margin-top: 3rem;
    padding: 2rem;
    background: var(--bg-card);
    border-top: 1px solid var(--border);
    text-align: center;
  }
  .footer p { margin-bottom: 1rem; font-size: 1rem; }
  .footer-nav { display: flex; justify-content: center; gap: 2rem; }
  .footer-nav a { font-size: 1rem; font-weight: 600; color: var(--text-muted); transition: color 0.2s ease; }
  .footer-nav a:hover { color: var(--primary); }

  @media (max-width: 768px) {
    .container { padding: 0 1rem; }
    .header { flex-direction: column; gap: 1rem; padding: 1rem; }
    .hero-title { font-size: 1.75rem; }
    .hero-desc { font-size: 1rem; }
    .grid-layout { grid-template-columns: 1fr; }
    .section-title { font-size: 1.25rem; }
    .article-card { padding: 1rem; }
    .category-card { padding: 1.5rem; }
  }
</style>
