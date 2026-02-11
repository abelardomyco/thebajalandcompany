# SEO — The Baja Land Company

Improve or implement SEO for this site. Use **real content only** from `content/` and `content/_meta.json`.

Do the following (implement what exists in the codebase; add what’s missing):

1. **Meta and document**
   - Unique `<title>` and `<meta name="description">` per page (home, about, blog, each post), derived from `content/` copy.
   - Canonical URLs for each page.

2. **Social and sharing**
   - Open Graph (og:title, og:description, og:image, og:url) and Twitter Card tags.
   - Use images from `public/images/` (e.g. logo or a gallery image) for og:image; no placeholder URLs.

3. **Technical**
   - `sitemap.xml` (all public pages: home, about, blog, blog posts).
   - `robots.txt` allowing crawling and pointing to sitemap.

4. **Structured data**
   - Consider JSON-LD for: LocalBusiness or RealEstateAgent (name, area served: Baja California, Mexico), and Article for blog posts (title, date, author from frontmatter).

5. **Content and UX**
   - Semantic HTML (headings, landmarks); ensure key phrases from `content/` (e.g. “land in Baja California”, “fideicomiso”) appear where appropriate for relevance.

Return a short checklist of what was added or changed and any env or config the user must set (e.g. base URL).
