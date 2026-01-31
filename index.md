---
layout: default
title: Coder Wealth
---

<style>
  /* CSS VARIABLES */
  :root {
    --primary: #2563eb;
    --primary-hover: #1d4ed8;
    --secondary: #64748b;
    --accent: #0d6efd;
    --bg-body: #f8f9fa;
    --bg-card: #ffffff;
    --text-main: #212529;
    --text-muted: #6c757d;
    --border: #e5e7eb;
    --radius: 8px;
    --shadow: 0 4px 6px rgba(0, 0, 0, 0.05);
    --transition: 0.2s ease-in-out;
  }

  /* BASE STYLES */
  * { box-sizing: border-box; margin: 0; padding: 0; }
  body {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
    background-color: var(--bg-body);
    color: var(--text-main);
    line-height: 1.6;
    -webkit-font-smoothing: antialiased;
  }
  a { color: var(--primary); text-decoration: none; transition: color var(--transition); }
  a:hover { color: var(--primary-hover); }

  /* CONTAINER */
  .container { max-width: 1200px; margin: 2rem auto; padding: 0 1rem; }

  /* HEADER */
  header {
    background: var(--bg-card);
    padding: 1.5rem 2rem;
    border-bottom: 2px solid var(--border);
    display: flex;
    justify-content: space-between;
    align-items: center;
    box-shadow: var(--shadow);
  }
  .logo {
    font-size: 1.5rem;
    font-weight: 800;
    color: var(--text-main);
    letter-spacing: 2px;
    text-transform: uppercase;
  }
  .nav-links { display: flex; gap: 2rem; }
  .nav-links a {
    font-size: 1rem;
    font-weight: 600;
    text-transform: uppercase;
    letter-spacing: 0.05em;
    color: var(--text-muted);
  }

  /* HERO */
  .hero {
    text-align: center;
    padding: 4rem 2rem;
    background: linear-gradient(135deg, var(--primary), var(--accent));
    color: #ffffff;
    border-radius: var(--radius);
    margin-bottom: 3rem;
  }
  .hero h1 { font-size: 2.5rem; font-weight: 800; margin-bottom: 1rem; }
  .hero p { font-size: 1.25rem; opacity: 0.95; max-width: 700px; margin: 0 auto 1.5rem; }
  .hero-btn {
    display: inline-block;
    background: #ffffff;
    color: var(--primary);
    padding: 1rem 2.5rem;
    border-radius: 9999px;
    font-weight: 700;
    font-size: 1.25rem;
    text-transform: uppercase;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    margin-top: 2rem;
    transition: transform 0.2s;
  }
  .hero-btn:hover { transform: translateY(-2px); box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); }

  /* SECTION TITLES */
  .section-title {
    font-size: 1.75rem;
    font-weight: 700;
    color: var(--text-main);
    margin: 2.5rem 0 1.5rem 0;
    padding-bottom: 0.75rem;
    border-bottom: 3px solid var(--primary);
  }

  /* GRID LAYOUT */
  .grid-layout { display: grid; grid-template-columns: 2fr 1fr; gap: 2rem; }
  @media (max-width: 900px) { .grid-layout { grid-template-columns: 1fr; gap: 1rem; } }

  /* ARTICLE LIST */
  .article-list { display: grid; grid-template-columns: 1fr 1fr; gap: 1.5rem; }
  @media (max-width: 768px) { .article-list { grid-template-columns: 1fr; gap: 1rem; } }

  .article-card {
    background: var(--bg-card);
    padding: 2rem;
    border: 1px solid var(--border);
    border-radius: var(--radius);
    transition: transform var(--transition), box-shadow var(--transition);
  }
  .article-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
    border-color: var(--primary);
  }
  .article-title {
    font-size: 1.35rem;
    font-weight: 700;
    margin-bottom: 0.75rem;
    line-height: 1.4;
  }
  .article-title a {
    color: var(--text-main);
    display: block;
  }
  .article-title a:hover { color: var(--primary); }
  .article-excerpt {
    font-size: 1rem;
    color: var(--text-muted);
    margin-bottom: 1.5rem;
    line-height: 1.6;
  }
  .read-more {
    font-size: 0.9rem;
    font-weight: 700;
    color: var(--primary);
    text-transform: uppercase;
    letter-spacing: 0.1em;
    display: inline-block;
  }
  .read-more::after { content: ' →'; margin-left: 0.5rem; }
  .read-more:hover { color: var(--primary-hover); }

  /* CATEGORY CARDS */
  .category-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 1.5rem; }
  .category-card {
    background: var(--bg-card);
    padding: 2rem;
    border: 1px solid var(--border);
    border-radius: var(--radius);
    text-align: center;
    transition: transform var(--transition), box-shadow var(--transition);
  }
  .category-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
    border-color: var(--primary);
  }
  .cat-icon { font-size: 2.5rem; margin-bottom: 1rem; display: block; }
  .cat-title {
    font-size: 1.25rem;
    font-weight: 700;
    margin-bottom: 0.5rem;
    color: var(--text-main);
  }
  .cat-desc {
    font-size: 1rem;
    color: var(--text-muted);
    margin-bottom: 1.5rem;
    line-height: 1.5;
  }
  .cat-link {
    display: inline-block;
    padding: 0.75rem 1.5rem;
    background: var(--primary);
    color: #ffffff;
    border-radius: 9999px;
    font-weight: 600;
    text-transform: uppercase;
    letter-spacing: 0.05em;
    transition: background var(--transition);
  }
  .cat-link:hover { background: var(--primary-hover); }

  /* FOOTER */
  footer {
    text-align: center;
    padding: 2rem;
    background: #f1f3f5;
    border-top: 1px solid var(--border);
    color: var(--text-muted);
  }
  .footer p { margin-bottom: 0.5rem; }
  .footer-links { display: flex; justify-content: center; gap: 2rem; margin-bottom: 0; }
  .footer-links a { font-weight: 600; color: var(--text-main); transition: color var(--transition); }
  .footer-links a:hover { color: var(--primary); }

  /* RESPONSIVE */
  @media (max-width: 768px) {
    .container { padding: 0 0.5rem; }
    header { flex-direction: column; gap: 1rem; text-align: center; padding: 1rem; }
    .nav-links { gap: 1rem; font-size: 0.9rem; justify-content: center; }
    .hero h1 { font-size: 1.75rem; }
    .hero p { font-size: 1rem; }
    .section-title { font-size: 1.4rem; margin: 2rem 0 1rem 0; }
    .article-card { padding: 1.5rem; }
    .article-title { font-size: 1.2rem; }
    .category-card { padding: 1.5rem; }
  }
</style>

<div class="container">

  <!-- HEADER -->
  <header>
    <div class="logo">CODERWEALTH</div>
    <nav class="nav-links">
      <a href="#tech">Tech</a>
      <a href="#investing">Investing</a>
      <a href="#education">Education</a>
      <a href="#tools">Tools</a>
    </nav>
  </header>

  <!-- HERO -->
  <section class="hero">
    <h1>Master DevOps & Financial Independence</h1>
    <p>Your definitive resource for building wealth through technology. High-level tutorials, proven investment strategies, and productivity tools for developers.</p>
    <a href="#articles" class="hero-btn">Start Learning</a>
  </section>

  <!-- LAYOUT: ARTICLES + CATEGORIES -->
  <div class="grid-layout">

    <!-- LEFT COLUMN: ARTICLES -->
    <section id="articles">
      <h2 class="section-title">Latest Articles</h2>
      <div class="article-list">

        <!-- ARTICLE 1: FIRE Strategy -->
        <div class="article-card">
          <h3 class="article-title"><a href="/_posts/invest/fire/2026/01/27/fire-strategy-tech-workers-2026/">FIRE Strategy for Tech Workers: Complete 2026 Guide</a></h3>
          <p class="article-excerpt">Achieve financial independence and retire early using your high developer salary and passive income streams.</p>
          <a class="read-more">Read More</a>
        </div>

        <!-- ARTICLE 2: Real Estate Investing -->
        <div class="article-card">
          <h3 class="article-title"><a href="/_posts/invest/realestate/2026/01/27/realestate-investing-tech-workers-2026/">Real Estate Investing for Tech Workers: Complete 2026 Guide</a></h3>
          <p class="article-excerpt">Build passive income through REITs, crowdfunding, turnkey rentals, and international properties.</p>
          <a class="read-more">Read More</a>
        </div>

        <!-- ARTICLE 3: Crypto & DeFi Strategies -->
        <div class="article-card">
          <h3 class="article-title"><a href="/_posts/invest/crypto/2026/01/27/crypto-defi-strategies-2026/">Crypto & DeFi Strategies for 2026: Complete Guide</a></h3>
          <p class="article-excerpt">Master blockchain investing, staking (5-14% APY), yield farming, and secure Web3 protocols.</p>
          <a class="read-more">Read More</a>
        </div>

        <!-- ARTICLE 4: Terraform IaC Guide -->
        <div class="article-card">
          <h3 class="article-title"><a href="/_posts/tech/terraform/2026/01/27/terraform-iac-complete-guide-2026/">Complete Terraform Guide: Infrastructure as Code (IaC) for 2026</a></h3>
          <p class="article-excerpt">Automate AWS, Azure, and GCP infrastructure. Master state management, modules, and CI/CD integration.</p>
          <a class="read-more">Read More</a>
        </div>

      </div>
    </section>

    <!-- RIGHT COLUMN: CATEGORIES -->
    <section>
      <h2 class="section-title">Categories</h2>
      <div class="category-grid">

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

</div>

<!-- FOOTER -->
<footer>
  <p>&copy; 2026 Coder Wealth. All rights reserved.</p>
  <div class="footer-links">
    <a href="https://twitter.com/coderwealth">Twitter</a>
    <a href="https://github.com/coderwealth">GitHub</a>
  </div>
</footer>
