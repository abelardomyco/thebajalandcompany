# Sales and lead capture

Add or improve **sales and lead capture** for The Baja Land Company. Use **real data only** — no mock submissions or fake CRM.

1. **Contact / lead form**
   - Ensure there is a clear contact or “inquiry” form (name, email, phone, message and/or property interest).
   - On submit: send to a real destination (e.g. email via API, form service like Formspree/Netlify Forms, or webhook to CRM). Document required env vars (e.g. `FORM_ENDPOINT`, `CONTACT_EMAIL`).
   - No mock “thank you” data: success state should reflect actual submit behavior (e.g. “We’ll contact you shortly” and optional redirect).

2. **CTAs**
   - Add or refine CTAs (e.g. “Inquire about this property”, “Schedule a call”) that point to the form or a real contact method (phone/email from `content/` if available).

3. **Optional integrations**
   - If integrating with a CRM (HubSpot, Salesforce, etc.) or email tool: use official APIs or webhooks; document required keys and webhook URLs in README or `.env.example`.
   - If storing leads in a DB: use a real database (e.g. Supabase, Neon); no mock or in-memory fake DB in production code.

4. **Compliance**
   - Do not store or transmit sensitive data (e.g. full SSN) unless required and secured; keep forms and storage minimal and compliant.

List what was added or changed and what the user must configure (env, form endpoint, CRM webhook).
