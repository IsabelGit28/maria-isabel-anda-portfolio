# Maria Isabel Anda Portfolio Website

Astro static portfolio website for Maria Isabel Anda's fully remote HR job search.

## Local Development

- Install dependencies: `npm install`
- Start dev server: `npm run dev`
- Build: `npm run build`
- Preview build: `npm run preview`

## Project Structure

- `src/pages/index.astro`: one-page portfolio route
- `src/components/`: reusable Astro components
- `src/data/portfolio.ts`: portfolio content arrays and case studies
- `src/styles/global.css`: full production styling converted from the Aura direction
- `public/resume-placeholder.txt`: temporary resume download placeholder
- `DESIGN-SYSTEM.md`: design system and future-page guidance

## Cloudflare Pages Setup

Recommended Cloudflare Pages settings after the GitHub repository exists:

- Framework preset: Astro
- Build command: `npm run build`
- Build output directory: `dist`
- Root directory: `/`
- Node version: current Cloudflare default is usually fine, but use Node 20+ if asked

## Blocked Before Deployment

These actions need Isabel's confirmation before I do them:

- GitHub account or organization to use
- Repository name and visibility
- Whether to create or use an existing dedicated GitHub SSH key
- Cloudflare account and zone
- Desired live URL or domain/subdomain
- Infrastructure note location, since `digitalgarden/4 TOOLS/Infrastructure.md` does not currently exist
- Explicit confirmation before any DNS, custom domain, token, SSH key, or Cloudflare project change

## Follow-Ups

- Replace `public/resume-placeholder.txt` with the final resume PDF.
- Add a professional portrait or abstract HR systems visual.
- Add anonymized case study visuals if they are safe to show publicly.
- Confirm which metrics should remain public.
- Decide final domain and Cloudflare Pages project name.
- Add analytics only after confirming the analytics provider and consent needs.
