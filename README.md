# My Tasks App

## Files
- `index.html` — Login page (Google, Microsoft, Zoho, Email)
- `app.html`   — Main task manager application
- `vercel.json` — Vercel deployment config

## Deploy to Vercel (5 minutes, free)

### Option A — Drag & Drop (easiest, no account needed)
1. Go to https://vercel.com/new
2. Sign up for a free account (use GitHub, Google, or email)
3. Click "Deploy" → choose **"Browse"** to upload files
4. Drag this entire folder into the upload area
5. Click Deploy — you'll get a live URL in ~30 seconds

### Option B — Vercel CLI
```bash
npm i -g vercel
cd mytasks-app
vercel
```
Follow the prompts. Your app will be live at a `.vercel.app` URL.

## Setting up real OAuth (optional)

### Google
1. Go to https://console.cloud.google.com
2. Create a project → APIs & Services → Credentials
3. Create OAuth 2.0 Client ID (Web application)
4. Add your Vercel URL to Authorized redirect URIs
5. Copy the Client ID into `index.html` where marked INTEGRATION POINT

### Microsoft
1. Go to https://portal.azure.com → Azure Active Directory → App registrations
2. New registration → add your Vercel redirect URI
3. Copy Application (client) ID into `index.html`

### Zoho
1. Go to https://api-console.zoho.com
2. Add Client → Server-based Applications
3. Set redirect URI to your Vercel URL
4. Copy Client ID into `index.html`
