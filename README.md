# Vet Feeding Calculator (Next.js + Supabase)

## 1) Create Supabase project
- Go to https://supabase.com → **Start your project** → create a free project.
- In the project, open **SQL Editor** → paste the contents of `supabase.sql` → **RUN**.
- Open **Table Editor** → click **diets** → **Import data** → upload `diet-seed.csv` → **Import**.

## 2) Get your Supabase keys
- In Supabase: **Project Settings** → **API** → copy **Project URL** and **anon public key**.

## 3) Configure the app
- Open `.env.local` and paste your values:
```
NEXT_PUBLIC_SUPABASE_URL=<paste project url>
NEXT_PUBLIC_SUPABASE_ANON_KEY=<paste anon key>
```

## 4) Run locally (optional)
```
npm install
npm run dev
# open http://localhost:3000
```

## 5) Deploy on Vercel
- Create a GitHub repo and upload all files from this folder.
- Go to https://vercel.com → **New Project** → Import your GitHub repo.
- In **Settings → Environment Variables**, add:
  - `NEXT_PUBLIC_SUPABASE_URL`
  - `NEXT_PUBLIC_SUPABASE_ANON_KEY`
- Click **Deploy**.

## Using the app
- Search a diet, enter weight & condition, click **Calculate**.
- Click **Buy on VetSource** to open the diet link.
