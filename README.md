# Coder Wealth - Build Wealth Through Code and Investing

## 🎯 Mission

Help developers build wealth through code, investing, and smart financial decisions.

## 📊 Content Strategy

### Niche Distribution
- **Technology (60%)** - Cloud, DevOps, Security, Database, SaaS
- **Finance (25%)** - Investing for Developers, Passive Income, Tax Planning
- **Education (10%)** - Certifications, Interview Prep, Learning Paths
- **Reviews (5%)** - CRM, Project Management, Developer Tools

### Why This Strategy?

**Maximum AdSense Revenue:**
- Technology (CPC: $20-50)
- Finance (CPC: $30-80)
- Education (CPC: $20-50)
- Reviews (CPC: $25-55)

**Developer-Targeted Audience:**
- Technical professionals with higher income
- People actively searching for solutions
- Purchasing decisions driven by technical needs
- High engagement with code-related content

## 📂 Project Structure

```
coderwealth.com/
├── _config.yml           # Jekyll configuration
├── _posts/              # All articles
│   ├── tech/           # 60% - Technology content
│   │   ├── cloud/      # AWS, Azure, GCP
│   │   ├── security/    # Cybersecurity
│   │   ├── devops/     # Kubernetes, CI/CD
│   │   └── database/   # SQL, NoSQL
│   ├── finance/         # 25% - Finance for Devs
│   │   ├── investing/   # US stocks, ETFs
│   │   ├── passive/    # Passive income
│   │   └── tax/        # Tax planning
│   ├── learn/           # 10% - Education
│   │   ├── cert/       # Certifications
│   │   ├── interview/   # Interview prep
│   │   └── roadmap/    # Learning paths
│   └── tools/           # 5% - Reviews
│       ├── crm/        # CRM reviews
│       ├── project/     # Project management
│       └── dev-tools/   # Developer tools
├── _layouts/            # Custom layouts (optional)
├── _includes/           # Custom includes (optional)
├── _sass/               # Custom styles (optional)
├── css/                  # Stylesheets
├── js/                   # JavaScript (optional)
├── images/               # Images
├── index.html            # Homepage
├── tech.html             # Tech index
├── invest.html           # Finance index
├── learn.html            # Education index
├── tools.html            # Tools index
├── about.html            # About page
├── .gitignore            # Git ignore
└── README.md             # This file
```

## 🚀 Getting Started

### For Readers

1. **Explore content by topic:**
   - Technology: `/tech/`
   - Finance: `/invest/`
   - Education: `/learn/`
   - Tools: `/tools/`

2. **Featured articles:**
   - Tech: Cloud computing, DevOps, cybersecurity
   - Finance: US stocks, ETFs, passive income
   - Education: Certifications, interview prep
   - Tools: CRM, project management software

### For Contributors

1. **Install Jekyll:**
   ```bash
   gem install jekyll bundler
   ```

2. **Clone repository:**
   ```bash
   git clone https://github.com/coderwealth/coderwealth.com.git
   cd coderwealth.com
   ```

3. **Install dependencies:**
   ```bash
   bundle install
   ```

4. **Run locally:**
   ```bash
   bundle exec jekyll serve
   ```

5. **Create new article:**
   - Add to `_posts/tech/`, `_posts/finance/`, etc.
   - Follow Jekyll front matter format
   - Use categories: `tech`, `finance`, `learn`, `reviews`

## 📝 Article Format

### Front Matter (YAML)

```yaml
---
layout: post
title: "Article Title Here"
date: 2026-01-27 04:00:00 -0300
categories: [tech]
tags: [cloud, aws, best-practices]
author: "Clever Weekly"
description: "Short description for SEO (160 chars max)"
image: /images/tech/article-image.jpg
---
```

### Article Structure

- **Title** - SEO optimized, includes keywords
- **Table of Contents** - For navigation
- **Introduction** - What reader will learn
- **Body** - H2/H3 structure with code blocks
- **Related Articles** - Internal links (reduces bounce rate)
- **Call to Action** - Subscribe (builds email list)

## 🔧 Development

### Tech Stack

- **Static Site Generator:** Jekyll
- **Hosting:** GitHub Pages (free, HTTPS auto)
- **Domain:** coderwealth.com (owned)
- **CSS Framework:** Bootstrap (responsive)
- **Syntax Highlighting:** Rouge
- **Comments:** Disqus (optional)

### Setup

1. **GitHub Pages:**
   - Repository: `coderwealth/coderwealth.com`
   - Settings > Pages > Source: `main` branch
   - Custom domain: `coderwealth.com`

2. **Domain:**
   - Registered via Namecheap/Godaddy
   - DNS configured to point to GitHub Pages
   - CNAME file created with `coderwealth.com`

3. **Jekyll:**
   - Ruby version: 3.x
   - Plugins: `jekyll-sitemap`, `jekyll-seo-tag`
   - Build time: ~1 minute

## 📊 SEO Strategy

### Keywords

**High CPC Tech Keywords:**
- Cloud computing, AWS certification, Kubernetes, DevOps, Cybersecurity

**High CPC Finance Keywords:**
- Investing for developers, US stocks for Brazilians, Passive income, Tax planning

### Optimization

- **Title tags:** Include primary keyword
- **Meta descriptions:** 160 chars max, compelling
- **URL structure:** `coderwealth.com/tech/aws-certification-guide`
- **Internal linking:** Related articles reduce bounce rate
- **Image alt text:** Include keywords
- **Mobile responsive:** Bootstrap handles this

### Performance

- **Site speed:** Fast (static site, no database)
- **Mobile:** Responsive (Bootstrap 5)
- **HTTPS:** Auto (GitHub Pages)
- **CDN:** GitHub Pages uses Fastly

## 💰 Monetization

### AdSense

- **Approval required:** Must have original content + traffic
- **CPC range:** $20-80 (depending on niche)
- **Placement:** In-article, sidebar
- **Compliance:** AdSense policies followed

### Alternative Revenue

- **Affiliate marketing:** SaaS, cloud hosting, tools
- **Sponsorships:** Tech companies, financial services
- **Digital products:** Courses, templates (future)

## 📈 Growth Strategy

### Content Plan (First 90 Days)

**Month 1:**
- 30 articles total (tech: 18, finance: 7, learn: 3, tools: 2)
- Focus on high CPC keywords
- Build internal linking structure

**Month 2:**
- 30 more articles
- Start email list
- Promote on tech forums

**Month 3:**
- 30 more articles
- Apply for AdSense (with 30+ articles)
- Social media promotion

### Traffic Goals

- **Month 1:** 0-1,000 pageviews
- **Month 2:** 1,000-5,000 pageviews
- **Month 3:** 5,000-10,000 pageviews
- **Month 6:** 10,000+ pageviews (apply AdSense)

## 🛡 Maintenance

### Weekly

- **Content:** 3-5 new articles
- **SEO:** Check Google Search Console
- **Analytics:** Review traffic, top pages

### Monthly

- **Backup:** Full repository backup
- **Audit:** Check for broken links
- **Review:** Performance, speed
- **Update:** Jekyll, plugins, dependencies

## 🤝 Contributing

### Writers

1. Fork repository
2. Create branch (`git checkout -b your-article`)
3. Add article to `_posts/` (follow format)
4. Commit (`git commit -m "Add article"`)
5. Push branch (`git push origin your-article`)
6. Create Pull Request

### Developers

1. Fork repository
2. Create branch (`git checkout -b feature-x`)
3. Make changes
4. Test locally
5. Commit and push
6. Create Pull Request

## 📄 License

Content is copyrighted. All rights reserved.

## 📧 Contact

- **Email:** contact@coderwealth.com
- **GitHub:** https://github.com/coderwealth
- **Twitter:** https://twitter.com/coderwealth
- **Discord:** (coming soon)

## 🎓 Disclaimer

All financial content is for educational purposes only. Not financial advice. Always do your own research before investing.

---

**Built with Jekyll & GitHub Pages**
**© 2026 Coder Wealth - All Rights Reserved**
