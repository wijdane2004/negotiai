# NegotiAI

Autonomous B2B supplier negotiation SaaS — bilingual (FR/EN), powered by Groq AI.

## Deploy to Vercel (free, permanent)

### Option A — Drag & Drop (fastest)
1. Run `npm install && npm run build` locally → upload the `dist/` folder to [vercel.com/new](https://vercel.com/new)

### Option B — GitHub (recommended, auto-deploys on every push)
1. Push this folder to a new GitHub repository
2. Go to [vercel.com/new](https://vercel.com/new) → Import your repo
3. Vercel auto-detects Vite — no config needed
4. Add your environment variable:
   - Key: `VITE_GROQ_API_KEY`
   - Value: your key from [console.groq.com](https://console.groq.com) (free)
5. Click **Deploy** — done!

## Run locally

```bash
npm install
cp .env.example .env.local   # then fill in your Groq API key
npm run dev
```

## Stack
- React 19 + Vite 7 + TypeScript
- Tailwind CSS v4 + shadcn/ui
- Groq AI (llama-3.3-70b-versatile) — free tier available
- localStorage (no backend, no database)
- wouter for routing, Recharts for analytics

## Features
- Bilingual FR/EN toggle
- Dashboard with KPIs and analytics
- Supplier management & comparison
- AI-generated negotiation emails
- Multi-round supplier AI simulation with counter-offers
- Negotiation progress tracker with agreement detection
