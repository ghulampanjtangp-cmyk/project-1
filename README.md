Interval — Responsive Landing Page
A single-page, fully responsive landing page for Interval, a focus-timer product. Built as a self-contained `index.html` (no build step, no dependencies) so it can be dropped into any static host.
**Live demo:** https://ghulampanjtangp-cmyk.github.io/project-1/
Screenshots: add desktop, tablet, and mobile screenshots here (see "Taking screenshots" below)
What's included
Hero section — headline, subhead, primary CTA, and a live working countdown timer as the hero visual.
Feature sections — a spotlighted "rhythm" explainer plus two supporting feature blocks (asymmetric layout, not identical cards).
Interactive element — the hero timer actually counts down (Start / Pause / Reset), with a progress bar and status text that updates live. This is a real interaction, not just a hover effect.
Testimonial band, pricing/CTA band, and footer with secondary links.
Semantic HTML — `header`, `nav`, `main`, `section`, `article`, `footer`, `blockquote`, `cite`.
Meta tags — `<title>`, meta description, and Open Graph title/description tags in `<head>`.
Responsive breakpoints at 900px (tablet: stacked hero/feature grids) and 640px (mobile: collapsed nav, tighter spacing).
Visible keyboard focus states and a `prefers-reduced-motion` fallback.
Tech stack
Plain HTML, CSS, and vanilla JavaScript. No frameworks, no build tools, no npm install. Fonts (Fraunces, Work Sans, IBM Plex Mono) are loaded from Google Fonts via a `<link>` tag.
Running it locally
Just open `index.html` in a browser — there's nothing to install or compile.
If you'd rather serve it (recommended for testing on mobile devices on your network):
```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```
Deploying (for the live demo link)
Easiest option — GitHub Pages:
Push this repo to GitHub.
Go to Settings → Pages.
Under "Build and deployment," set Source to "Deploy from a branch," pick your `main` branch and `/ (root)` folder.
Save. Your live URL will be `https://<your-username>.github.io/<repo-name>/`.
Alternatives: drag-and-drop the folder into Netlify Drop, or run `vercel` in the folder with the Vercel CLI.
Taking screenshots
Once deployed (or running locally):
Desktop: open the page at a wide window (~1440px) and use your OS screenshot tool, or your browser's DevTools → Device Toolbar → "Capture screenshot."
Tablet / Mobile: in Chrome/Edge DevTools, open Device Toolbar (Ctrl/Cmd+Shift+M), pick "iPad Air" and "iPhone 14," then capture a screenshot for each.
Save them into a `screenshots/` folder in the repo (e.g. `screenshots/desktop.png`, `screenshots/tablet.png`, `screenshots/mobile.png`) and reference them at the top of this README.
Customizing for a different product
Everything specific to "Interval" lives in the copy and the timer widget:
Swap headline, subhead, feature copy, and testimonial text in `index.html`.
The color tokens are CSS variables at the top of the `<style>` block (`--bg`, `--ink`, `--accent`, `--gold`) — change these to re-theme the whole page.
The hero timer widget can be removed or replaced with any other interactive element (an image carousel, a calculator, a before/after slider) without touching the rest of the layout.
License
Use freely for your own project.
