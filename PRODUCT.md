# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

- **Primary:** Recruiters and hiring managers evaluating Talha for senior backend/engineering roles
- **Secondary:** Collaborators and open-source contributors seeking technical credibility
- **Tertiary:** Students and general public learning about backend engineering and AI/ML

## Product Purpose

Talha Asghar's professional portfolio and personal website. The primary job is to get Talha hired for senior backend engineering roles by demonstrating technical depth, architectural thinking, and real-world impact. Secondary jobs: establish authority in distributed systems and AI/ML, share knowledge through blog posts and publications.

## Positioning

Unlike generic developer portfolios that list technologies, this site demonstrates engineering discipline through its own construction. The precision of the design signals the precision of the work. Talha's unique combination of 4+ years in distributed systems (Galera, ClickHouse, Redis, MySQL clusters) with a Master's in AI/ML from NUST positions him at the intersection of production engineering and applied research.

## Operating Context

- **Deployment:** GitHub Pages with Jekyll static site generator
- **Theme:** al-folio (academic portfolio theme, vendored locally)
- **Content sources:** YAML data files for CV/publications, Markdown for blog/posts, Jekyll Scholar for bibliography
- **Blog topics:** Backend engineering, data engineering, FOSS, Linux, fediverse
- **Contact:** Email and LinkedIn (stated in contact note)

## Capabilities and Constraints

- **Must preserve:** All academic features (publications with BibTeX, CV with timeline, teaching pages)
- **Must preserve:** Jekyll Scholar bibliography integration
- **Must preserve:** Dark/light mode toggle
- **Must preserve:** Responsive design (mobile/tablet/desktop)
- **Must preserve:** GitHub Pages compatibility (no server-side processing)
- **Constraint:** Cannot remove or modify Jekyll plugins (user explicitly excluded)
- **Constraint:** Must maintain existing URL structure and navigation
- **Technical:** Bootstrap 4 + MDB, jQuery 3.6.0, Font Awesome, Tabler Icons

## Brand Commitments

- **Name:** Talha Asghar
- **Voice:** Professional, technically rigorous, approachable. Not corporate-stiff, not casual-playful.
- **Personality:** Precision engineer — deliberate, purposeful, disciplined. Every element has a reason.
- **Tagline:** "Senior Software Engineer | Architecting Scalable Backend Systems & Leading AI/ML/DL Initiatives"
- **Contact note:** "The best way to reach me out is through given email or linkedin."

## Evidence on Hand

- **Profile image:** `assets/img/prof_pic.png` (rectangular headshot)
- **CV data:** `_data/cv.yml` (education, work, skills, certificates, awards, publications)
- **Publications:** BibTeX files in `_bibliography/` (Google Scholar integration)
- **Blog posts:** Markdown files in `_posts/` with Jupyter notebook support
- **Projects:** YAML data in `_data/projects.yml`
- **PDF resume:** `talhaasghar-resume.pdf`

## Product Principles

1. **Precision over decoration** — Every design element must justify its existence. No decorative gradients, no whimsical animations, no generic patterns.
2. **Content is the product** — The portfolio's value is the work it presents, not the design itself. Design serves content, never competes with it.
3. **Engineering discipline signals engineering quality** — The site's construction quality reflects the engineer's construction quality. Consistency, attention to detail, and deliberate choices matter.
4. **Accessible by default** — Keyboard navigation, screen readers, contrast ratios, and reduced motion are not afterthoughts.
5. **Maintainable over clever** — Simple, clear CSS tokens and patterns that can be understood and modified without specialized knowledge.

## Accessibility & Inclusion

- Keyboard navigation through all interactive elements
- Visible focus indicators
- Screen reader compatible landmarks and labels
- Contrast ratios: body text ≥4.5:1, large text ≥3:1
- Reduced motion support via `prefers-reduced-motion`
- Responsive design for mobile/tablet/desktop
