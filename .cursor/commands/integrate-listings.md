# Integrate listing services (Zillow, Redfin, etc.)

Plan or implement integrations for property listings for The Baja Land Company. **No mock data** — use real APIs, feeds, or official syndication where available.

1. **Research and choose**
   - Check Zillow, Redfin, and any Baja/Mexico MLS or listing APIs or syndication programs (e.g. Zillow Partner Program, Realtor.com, or local Baja MLS if documented).
   - Prefer official APIs or feed specs; document requirements (keys, webhooks, feed URLs).

2. **Implementation options**
   - **API/feed:** If an API or RSS/XML feed exists: add server-side or build-time fetch, normalize to a single listing shape, render on the site. Store API keys or feed URLs in env (e.g. `ZILLOW_*`, `LISTINGS_FEED_URL`); document in README or `.env.example`.
   - **Embed/widget:** If only embeds or iframes are available: add the official embed code and document where to get it and any account setup.
   - **Manual/CSV:** If no API: define a simple format (e.g. JSON or CSV in `content/listings/` or a CMS) and a script or page that reads it and displays listings. No fake listings.

3. **Display**
   - Listings should use real data only. Property images can come from `public/images/` or from the feed; do not invent listing text or photos.
   - Link to source (Zillow/Redfin listing URL) when applicable.

Summarize what was implemented, what’s left (e.g. “add ZILLOW_API_KEY”), and where keys/feeds are configured.
