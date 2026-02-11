# Full website checklist — The Baja Land Company

Run through this checklist for the site. Use **real content** from `content/` and **real data only** (no mocks). For each item, implement if missing or confirm if already done.

## 1. SEO
- [ ] Per-page `<title>` and `<meta name="description">` from `content/`
- [ ] Open Graph and Twitter Card tags; og:image from `public/images/`
- [ ] `sitemap.xml` and `robots.txt`
- [ ] JSON-LD (e.g. LocalBusiness/RealEstateAgent, Article for blog)
- [ ] Canonical URLs

## 2. Integrations (listings)
- [ ] Research: Zillow, Redfin, or Baja/Mexico listing feeds or APIs
- [ ] Implement: feed/API fetch or embed; env for keys/URLs; document in README
- [ ] Listings displayed from real source only

## 3. Sales and leads
- [ ] Contact/lead form with real submit endpoint (email, form service, or CRM webhook)
- [ ] CTAs (e.g. “Inquire”) point to form or real contact
- [ ] Env/docs for FORM_ENDPOINT, CONTACT_EMAIL, or CRM keys

## 4. Property management
- [ ] Property data from `content/` or real listing feed (no mock)
- [ ] Listing UI: name, description, images from `public/images/`, status, CTA
- [ ] Optional: detail page per property, filters, status (available/pending/sold)

## 5. Content and assets
- [ ] All copy from `content/`; no hardcoded mock text
- [ ] All images from `public/images/` or listing feed; no fake images
- [ ] Blog posts from `content/blog/*.md` with frontmatter

## 6. Technical
- [ ] No mock or fake data in codebase; real config (env, CMS, API) documented
- [ ] Base URL / domain config for sitemap, canonicals, OG

Reply with: what’s done, what’s missing, and next steps (in order of priority).
