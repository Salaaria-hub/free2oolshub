# FreeToolsHub — Deployment Guide

## Current Status
Site is ready to deploy on Cloudflare Pages free tier.
Temporary URL: https://freetoolzhub.pages.dev
Custom domain (later): freetoolshub.com (not purchased yet)

## Pre-Deployment Checklist
- [ ] All 14 files present (5 root HTML + 3 SEO files + 6 blog files)
- [ ] Formspree ID replaced in contact.html (search for "xxxxxxxx")
- [ ] All tools tested locally at http://localhost:8080
- [ ] Mobile responsive verified
- [ ] Browser console has no errors

## Deploy to Cloudflare Pages (10 minutes)
1. Go to https://pages.cloudflare.com and sign up (free)
2. Click "Workers & Pages" → "Create application" → "Pages" → "Upload assets"
3. Project name: freetoolshub
4. Drag ALL files from inside the Freetoolshub folder (NOT the folder itself)
   Correct structure on Cloudflare:
   /index.html
   /about.html
   /blog/index.html
   /blog/compress-images-without-losing-quality.html
   etc.
5. Click "Deploy site"
6. Live URL: https://freetoolzhub.pages.dev

## Post-Deployment (Day 1)
1. Test all 8 tools at https://freetoolzhub.pages.dev
2. Test mobile view
3. Submit to Google Search Console:
   - Add property: https://freetoolzhub.pages.dev
   - Verify ownership
   - Submit sitemap: https://freetoolzhub.pages.dev/sitemap.xml
   - Request indexing for homepage

## Custom Domain (Month 2-3)
1. Buy domain (~₹750/year) from Cloudflare Registrar or Namecheap
2. Cloudflare Pages → project → Custom domains → Add domain
3. Follow DNS instructions (auto if domain is on Cloudflare)
4. Replace "freetoolzhub.pages.dev" with new domain in ALL files
5. Re-deploy on Cloudflare Pages
6. Old .pages.dev URLs auto-redirect to new domain

## AdSense Application (Month 3)
- Wait 2-3 months after deploy
- Build organic traffic (100+ visits/month minimum)
- Apply at https://adsense.google.com
- After approval:
  - Update ads.txt with Google's provided line
  - Uncomment AdSense script in index.html <head>
  - Replace 3 ad-placeholder divs with actual ad unit code
