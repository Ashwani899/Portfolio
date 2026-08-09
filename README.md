# Ashwani Singhal — Portfolio

A single-file, self-contained portfolio site — no build step, no dependencies to install. Open `index.html` and it works.

**Live site:** _add your URL here once deployed (see [Deploy](#deploy) below)_

---

## What's inside

One HTML file with everything embedded — profile photo and résumé PDF are both inlined as base64, so there's nothing else to host or link.

| Section | What it shows |
|---|---|
| **About** | Bio, education, and quick-fact stats (students reached, registrations driven, apps shipped, certifications) |
| **Projects** | ResumeForge AI and AI Study Assistant in full detail — live demo / code links, tech stack, an architecture pipeline diagram, challenges, and a roadmap, each behind tabs. Plus lighter cards for the two Techfest sites. |
| **GitHub Stats** | Live cards from the GitHub API (stars, commits, top languages) — no manual updating needed |
| **Skills** | Grouped badge pills: languages, AI/LLM tooling, frontend & backend, cloud & DevOps, practices |
| **Certifications** | Grouped by category, each card linking to the real verification page |
| **Leadership** | GeeksforGeeks Campus Mantri + Techfest, IIT Bombay Ambassador roles |
| **Resume** | Thumbnail preview + one-click PDF download (embedded, works offline) |
| **Contact** | Email with copy-to-clipboard, social links |

## Built with

Plain HTML, CSS, and vanilla JavaScript — no framework, no bundler.

- **Fonts:** Space Grotesk (display), IBM Plex Sans (body), IBM Plex Mono (labels/data) via Google Fonts
- **Live data:** [github-readme-stats](https://github.com/anuraghazra/github-readme-stats) for the GitHub Stats section
- **Interactivity:** `IntersectionObserver` for scroll-reveal and nav-spy, no other JS dependencies
- Fully responsive (mobile hamburger nav, single-column stacking below 860px), respects `prefers-reduced-motion`, and degrades gracefully with JavaScript disabled (`<noscript>` fallback keeps content visible)

## Deploy

Any static host works since it's one file. Pick whichever's easiest:

**GitHub Pages**
1. Create a repo (e.g. `portfolio` or `<your-username>.github.io`)
2. Add this `index.html` to the root and push
3. Repo → Settings → Pages → deploy from the `main` branch → done

**Vercel / Netlify**
- Drag the `index.html` file onto [vercel.com/new](https://vercel.com/new) or [app.netlify.com/drop](https://app.netlify.com/drop) — no config needed

**Local preview**
```bash
# just open it directly
open index.html        # macOS
start index.html        # Windows
# or serve it
python3 -m http.server 8000
```

## Customizing

Everything lives in one file, organized top to bottom in the order sections appear on the page.

- **Photo / résumé PDF** — both are base64 data URIs (`src="data:image/jpeg;base64,..."` and `href="data:application/pdf;base64,..."`). Replace by re-encoding a new file (`base64 -i yourfile.jpg`) and swapping the string, or ask Claude to regenerate the page with new files.
- **Colors / type** — all design tokens are CSS custom properties at the top of the `<style>` block (`:root { --bg, --ink, --indigo, --amber, ... }`). Change once, applies everywhere.
- **Projects** — each project is one `<article class="project-card">` block under `#projects`. Tab content lives in `.tabs__panel` divs right below the tab buttons.
- **Live demo links** — currently shown as "Coming soon" (disabled) for all four projects since none are deployed yet. Once a project is live, swap the `<span class="btn btn--disabled">` for an `<a>` tag with the real URL.
- **Screenshots** — the project preview boxes (`.mockup__stage`) currently hold illustrative placeholder SVGs, clearly labeled "Preview mockup." Replace with `<img src="your-screenshot.png" alt="...">` once real screenshots exist.
- **GitHub Stats username** — search `username=Ashwani899` and replace if this ever needs to point elsewhere.

## Known TODOs

- [ ] Deploy ResumeForge AI and AI Study Assistant, then swap their "Coming soon" buttons for real live-demo links
- [ ] Replace the two placeholder project mockups with real screenshots once deployed
- [ ] Enable GitHub Pages on the `Techfest-3D` and `Techfest-Synthesis` repos (both already have `index.html` at the root — it's a one-click Settings change) and link them as live demos too
- [ ] Update the "Open to Fall '26 roles" status pill in the nav as availability changes

## Browser support

Modern evergreen browsers (Chrome, Firefox, Safari, Edge). Uses CSS Grid, `backdrop-filter`, and `IntersectionObserver` — all standard since ~2017, no polyfills needed.

## License

© 2026 Ashwani Singhal. Feel free to fork the structure for your own portfolio — swap the content for yours.
