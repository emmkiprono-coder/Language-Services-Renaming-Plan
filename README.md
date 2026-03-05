# Language Services Naming Competition — Submission Portal

Advocate Health Language Services team naming submission form. Built with React + Vite + Tailwind CSS, data stored in JSONBin.io.

## Setup

```bash
# 1. Install dependencies
npm install

# 2. Configure environment
cp .env.example .env
# Edit .env with your JSONBin credentials (see below)

# 3. Run locally
npm run dev
```

## JSONBin Setup

1. Sign up at [jsonbin.io](https://jsonbin.io) (free)
2. Create a new bin — initialize with `[]`
3. Copy the **Bin ID** and your **X-Access-Key**
4. Add them to `.env`:
   ```
   VITE_JSONBIN_BIN_ID=your_bin_id
   VITE_JSONBIN_API_KEY=your_api_key
   ```

## Deploy to Vercel

```bash
# Option A: Vercel CLI
npm i -g vercel
vercel

# Option B: GitHub integration
# 1. Push this repo to GitHub
# 2. Go to vercel.com → New Project → Import your repo
# 3. Add environment variables in Vercel dashboard:
#    VITE_JSONBIN_BIN_ID and VITE_JSONBIN_API_KEY
# 4. Deploy
```

**Important:** Add `VITE_JSONBIN_BIN_ID` and `VITE_JSONBIN_API_KEY` as environment variables in the Vercel project settings.

## Data Format

Each submission is stored as:
```json
{
  "fullName": "Jane Doe",
  "department": "Interpretation",
  "proposedName": "BridgePoint",
  "rationale": "...",
  "unification": "...",
  "realWorldTest": "...",
  "culturalSignificance": "...",
  "tagline": "...",
  "submittedAt": "2026-03-10T14:30:00.000Z"
}
```
