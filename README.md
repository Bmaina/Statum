# Statum — Landing Page

A single-file, dependency-free landing page for Statum. No build step required.

## What's inside

`index.html` — the entire site (HTML, CSS, and JS in one file). Fonts (Space Grotesk,
IBM Plex Sans, IBM Plex Mono) load from Google Fonts via CDN; everything else is
self-contained.

## Before you deploy — placeholders to swap

- **Email address**: the "Request early access" and "Talk to the founder" buttons
  link to `maina.anu@gmail.com`. Replace with your real address (search for
  `maina.anu@gmail.com` in `index.html`, two occurrences).
- **Domain / title tag / meta description**: update if you register a real domain.
- **Favicon**: none is set. Add a `<link rel="icon" ...>` in `<head>` if you want one.

## Deploy for free — pick one

**Netlify (easiest, drag-and-drop)**
1. Go to https://app.netlify.com/drop
2. Drag the `statum-landing` folder (or just `index.html`) onto the page
3. Live instantly on a `*.netlify.app` URL; add a custom domain later for free

**Vercel**
1. `npm i -g vercel` (or use the Vercel dashboard's drag-and-drop import)
2. From this folder, run `vercel` and follow the prompts
3. Live on a `*.vercel.app` URL

**GitHub Pages**
1. Create a new GitHub repo, push this folder's contents to it
2. Repo Settings → Pages → Deploy from branch → `main` / root
3. Live at `https://<your-username>.github.io/<repo-name>/`
   (rename `index.html` — already named correctly — no changes needed)

**Cloudflare Pages**
1. https://pages.cloudflare.com → Create a project → Direct upload
2. Drag in this folder
3. Live on a `*.pages.dev` URL

## Notes

- Fully responsive (desktop → mobile), with a working mobile menu.
- Respects `prefers-reduced-motion`.
- No analytics, tracking, or forms wired up — the CTA buttons are `mailto:` links
  by design, so there's no backend to stand up before this is live.
