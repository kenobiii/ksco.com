# Ken Silva Co. — kensilvaco.com
### Personal Brand Website & Consultancy Hub
**Version 4.0 | Built April 2026**

---

## ⚠️ Important — Framework Notice

This is a **plain React + Vite** project. Do **not** use Tanstack Start, Next.js, Remix, or any other framework. If you are using an AI coding assistant (Copilot, Claude Code, etc.), tell it explicitly:

> "This is a React + Vite project. Use the existing package.json, vite.config.js, and src/main.jsx. Do not change the framework."

---

## What This Is

A single-page React application for Ken Silva Co. Fully mobile responsive, SEO-ready, deployable to kensilvaco.com via Vercel.

---

## File Structure

```
kensilvaco/
├── index.html
├── package.json
├── vite.config.js
├── vercel.json          ← Vercel deployment config
├── public/
│   ├── favicon.svg
│   └── og-image.svg
└── src/
    ├── main.jsx
    └── KenSilvaCo_v4.jsx
```

---

## Tech Stack

- React 18
- Vite 5
- Inline CSS / CSS-in-JSX
- Google Fonts
- Hosting: Vercel
- Domain: kensilvaco.com
- Email: ken@kensilvaco.com

---

## Local Setup

**1. Install Node.js** — nodejs.org (LTS version)

**2. Create Vite project**
```bash
npm create vite@latest kensilvaco -- --template react
cd kensilvaco
npm install
```

**3. Replace default files**

Delete `src/App.jsx`, `src/App.css`, `src/index.css` then copy:

| Your file | Destination |
|---|---|
| KenSilvaCo_v4.jsx | src/KenSilvaCo_v4.jsx |
| main.jsx | src/main.jsx |
| index.html | index.html |
| package.json | package.json |
| vite.config.js | vite.config.js |
| vercel.json | vercel.json |
| favicon.svg | public/favicon.svg |
| og-image.svg | public/og-image.svg |

After replacing package.json run `npm install` again.

**4. Run locally**
```bash
npm run dev
```
Visit http://localhost:3000

**5. Pre-deploy checklist**
- [ ] Boot sequence loads
- [ ] All nav links work
- [ ] Player Profile modal opens/closes
- [ ] Mission Log modal opens/closes
- [ ] Mobile menu works
- [ ] Contact links to ken@kensilvaco.com

---

## Deploy to Vercel

**1. Push to GitHub**
```bash
git init
git add .
git commit -m "kensilvaco v4.0"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/kensilvaco.git
git push -u origin main
```

**2. Import to Vercel**
1. Go to vercel.com, sign in with GitHub
2. Click Add New Project
3. Import kensilvaco repo
4. Vercel reads vercel.json automatically
5. Confirm: Framework = Vite, Build = npm run build, Output = dist
6. Click Deploy

**3. Connect domain**
1. Vercel → Project → Settings → Domains → Add kensilvaco.com
2. Add DNS records in your registrar:
   - A record: @ → 76.76.21.21
   - CNAME: www → cname.vercel-dns.com
3. SSL auto-provisions

---

## After Launch

- [ ] Send test email to ken@kensilvaco.com
- [ ] Check OG image at opengraph.xyz
- [ ] Submit to Google Search Console
- [ ] Update LinkedIn with kensilvaco.com

---

## Content Updates

Edit these constants at the top of KenSilvaCo_v4.jsx:

| Constant | Controls |
|---|---|
| STATS | Hero stats |
| SERVICES | Service cards |
| MISSIONS | Mission Log |
| SKILLS | Skill bars |
| CAREER | Career timeline |
| CLIENTS | Client grid + marquee |
| BOOT_LINES | Boot sequence text |

---

*Ken Silva Co. | kensilvaco.com | ken@kensilvaco.com*
