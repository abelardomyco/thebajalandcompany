# thebajalandcompany

Repo for The Baja Land Company website. A new site will be built here using the scraped content and assets from the original site.

## Content & assets

- **content/** — All site copy (source of truth). Use only this content; no mock data.
  - `homepage.md` — Welcome text, project blurbs, section headings, footer
  - `about.md` — About page body
  - `blog/` — Blog posts (Markdown with frontmatter: title, date, author)
  - `_meta.json` — Page list, image paths, and usage notes for building the new site
- **public/images/** — Images from the original site, ready for the new build
  - `logo.png` — Site logo
  - `gallery/` — Homepage gallery images (7)
  - `properties/` — Industrial Park and Lots section images

The new site should read from `content/` and `public/images/` only.

## Cursor: rules, commands, subagents

- **Rules** (`.cursor/rules/`): Project rule `baja-land-project.mdc` is always applied — content from `content/`, images from `public/images/`, no mock data; SEO, integrations (Zillow/Redfin), sales/leads, and property management are in scope.
- **Commands** (type `/` in Cursor chat):
  - `/seo` — Meta tags, OG, sitemap, robots.txt, structured data
  - `/integrate-listings` — Zillow, Redfin, or other listing feeds/APIs
  - `/sales-leads` — Contact form, lead capture, CTAs, CRM
  - `/property-management` — Property listings, status, detail pages
  - `/website-checklist` — Full checklist (SEO, integrations, sales, property, content)
- **Subagents** (`.cursor/agents/`): Delegate to specialists when needed:
  - `seo-specialist` — SEO improvements
  - `integrations-specialist` — Listing and lead-service integrations
  - `property-management-specialist` — Listings and property UI
