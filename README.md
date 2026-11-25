# 🛠️ FreeToolsHub

Free, 100% client-side online tools for images, PDFs, and everyday
utilities. No signup, no file uploads, no tracking.

**Live site:** https://free2oolshub.pages.dev (after deploy)

## Features
- 🖼️ Image Compressor, Resizer, Converter (JPG/PNG/WebP)
- 📄 Image to PDF, PDF Merge
- 📱 QR Code Generator
- 📝 Word Counter, Password Generator
- 📚 Blog with 5 SEO articles

## Tech Stack
- Pure HTML5 + CSS3 + Vanilla JavaScript (no frameworks)
- CDN libraries: pdf-lib, jsPDF, QRCode.js
- Deployed on Cloudflare Pages

## Local Development
1. Clone this repo
2. Run a local server:
   - `python -m http.server 8080` (Python 3)
   - OR `npx serve .` (Node.js)
3. Open http://localhost:8080

## Deployment

### Option 1: GitHub → Cloudflare (recommended, auto-deploy)
1. Push this repo to GitHub (see instructions below)
2. Go to https://dash.cloudflare.com → Workers & Pages → Create
3. Click "Pages" → "Connect to Git"
4. Select this repo
5. Build settings: leave defaults (no build command, output = /)
6. Click "Save and Deploy"
7. Every push to `main` branch auto-deploys

### Option 2: Wrangler CLI (manual)
```bash
npm install
npm run deploy
# First time: browser opens for Cloudflare login → authorize
# Subsequent deploys: no auth needed
```

### Push to GitHub
```bash
git remote add origin https://github.com/<your-username>/freetoolshub.git
git branch -M main
git push -u origin main
```
