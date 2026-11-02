# kiddie-bloom-api (PRIVATE repo)

Node payment/download API for Kiddie Bloom, deployed on Render. The public website lives in a separate repo.
- `index.js` — server (Razorpay orders, payment verification, one-time PDF download links)
- `catalog.cjs` — server-side price list (regenerate if you add shop items in the site's `src/data/initialData.ts`)
- `private-pdfs/<id>.pdf` — paid PDFs, sent only after payment
- `RENDER-SETUP.md` — Render settings and environment variables

Keep this repository PRIVATE. Never commit `.env` or service-account JSON.
Run locally: `npm install && npm start` (needs the variables from `.env.example` in the environment).
