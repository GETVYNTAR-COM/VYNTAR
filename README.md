# VYNTAR Marketplace Intelligence (MVP)

A simple MVP for capturing “Founder Edition” signups + viewing them in a dashboard.

## What’s live right now
- Landing page: https://getvyntar.vercel.app
- Supabase project: hfchmjmhkiqsibxtiwsk (UK)

## Current features
### Landing Page
- Founder signup form
- Writes to founder_signups table in Supabase

### Dashboard (next)
- Login (optional for MVP)
- View founder signups
- Filter/search
- Export CSV
- Mark signup status (new/contacted/approved)

## Database
### Table: founder_signups
Fields used by the form:
- name (text)
- email (text)
- phone (text, nullable)
- current_marketplace (text)
- monthly_revenue (text)
- biggest_pain_point (text)
- source (text)
- status (text)
- created_at (timestamp)

## Keys & security (IMPORTANT)
- Frontend uses *Publishable/Anon* key only (safe with RLS)
- *Secret key never goes in the browser*
- RLS must allow INSERT for landing page and SELECT for dashboard (authenticated or restricted)

## Deploy
- GitHub → Vercel (auto deploy on commit)

## Next build steps (Dashboard MVP)
1. Create /dashboard page (or route) with a table view
2. Pull rows from founder_signups
3. Add status update dropdown
4. Add export button

## Notes / Decisions log
- MVP focus: Founder signups + dashboard visibility
- Later: marketplace message ingestion + automation (Make.com)
