# Property management and listings

Implement or improve **property/listing management** for The Baja Land Company. All listing data must be **real** — from `content/`, `content/_meta.json`, or a real feed/CMS; no mock listings.

1. **Data source**
   - **Current:** Properties are described in `content/homepage.md` (e.g. Rancho La Escondida, Industrial Zone Park) and images in `public/images/` (see `content/_meta.json`).
   - Option A: Keep properties as content — add structured data (e.g. `content/properties/*.md` or a JSON file) with name, description, image paths, status (available/pending/sold), location, and link to contact form.
   - Option B: Connect a real listing feed or API (see `/integrate-listings` command); normalize and display those.

2. **UI**
   - Property listing page or section: show name, description, image(s) from `public/images/`, status, and CTA (e.g. “Inquire”) linking to contact form.
   - Optional: filters (e.g. by type: land, industrial), sort, and a detail page per property with gallery and full copy.

3. **Status and updates**
   - If status is stored (available/pending/sold), it should come from content or a real backend/CMS; do not hardcode fake statuses.

4. **Images**
   - Use only images under `public/images/` (gallery, properties) or from the chosen data source; no placeholder or fake images.

Summarize data source chosen, pages/components added or updated, and any env or content files the user must maintain.
