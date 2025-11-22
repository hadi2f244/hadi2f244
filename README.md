## Hadi Azaddel – DevOps & Platform Engineering

Public professional site and portfolio hosted on GitHub Pages: **https://hadiazaddel.ir**

### Focus
DevOps tooling maturity, automated infrastructure testing (Ansible + Molecule/Testinfra), delivery reliability, and actionable engineering metrics.

### Features
- Clean Jekyll site (minima theme + SEO & sitemap plugins)
- Structured sections: Home · Resume · Projects · Experience · Skills · Blog · Contact
- Embedded PDF resume (`resume.md`)
- Medium article summaries with JSON-LD Person & Article schema
- Custom domain + canonical URLs + robots.txt

### Structure
```
/_layouts/default.html      # Base layout + meta + navigation
/_includes/schema-person.html
/_includes/schema-articles.html
index.md                    # Home page
resume.md                   # Resume (embedded PDF)
projects/index.md
experience/index.md
skills/index.md
blog/index.md               # Medium summaries
contact/index.md
assets/css/custom.css       # Minimal styling
CNAME                        # Custom domain binding
robots.txt                   # Crawling directives
Hadi_Azaddel_CV_18Aban_1404.pdf
```

### Medium Articles Referenced
1. Ten Maturity Principles of DevOps Tooling
2. Ansible Code Testing – Part 2 – Writing Tests
3. Ansible Code Testing – Part 1 – Test Environment Automation

### Deployment
GitHub Pages builds from the `main` branch automatically. Custom domain handled by `CNAME` and DNS A records pointing to GitHub Pages IPs.

### Local Preview
Install Jekyll locally if desired:
```bash
gem install bundler jekyll
bundle init
echo 'gem "jekyll-seo-tag"\ngem "jekyll-sitemap"' >> Gemfile
bundle install
bundle exec jekyll serve
```
Browse: http://localhost:4000

### Analytics & Search
- Google Analytics: Uncomment `google_analytics:` in `_config.yml` and set GA4 Measurement ID.
- Search Console: Verify domain via DNS TXT record (preferred); submit sitemap at `/sitemap.xml`.
- Backlinks: Medium bio, LinkedIn profile, GitHub profile README linking to the site help ranking for "Hadi Azaddel".

### Custom Domain
`hadiazaddel.ir` is primary. Secondary `hadi2f244.ir` can 301 redirect at registrar. Use A records:
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

### Contact
Email: contact@hadiazaddel.ir  |  LinkedIn: https://www.linkedin.com/in/hadi-azaddel  |  Medium: https://medium.com/@m.h.azaddel  |  GitHub: https://github.com/hadi2f244

---
*Reliability, testability, and measurable engineering outcomes.*
