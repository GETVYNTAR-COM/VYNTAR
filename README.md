# VYNTAR Dashboard 

AI-powered marketplace intelligence dashboard for Facebook Marketplace sellers.

This is the **application dashboard**, not the public landing page.

---

## 🌐 Live URLs

- **Dashboard (App):** https://getvyntar.com  
- **Landing Page:** https://getvyntar.com/getvyntar

---

## 🧱 Tech Stack

- Vite + React + TypeScript
- Supabase (Database + Auth)
- Tailwind CSS
- Deployed on Vercel

---

## 🔐 Environment Variables (REQUIRED)

⚠️ **DO NOT put real API keys in this repo**

These variables must be added in **Vercel → Project → Settings → Environment Variables**

### Required variables:

```env
VITE_SUPABASE_URL=https://YOUR_PROJECT_ID.supabase.co
VITE_SUPABASE_ANON_KEY=YOUR_PUBLIC_ANON_KEY
