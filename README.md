# Óptica 20•20 — El Paso Landing Page

Single-page, bilingual (Spanish-default) landing page for the El Paso location at
8080 Gateway East, El Paso, TX 79907. Built to drive walk-in traffic and establish
that this location is genuinely open now, not just a Juárez brand reference.

Static site, no build step — open `index.html` directly or serve the folder with
any static file server.

## Status / open items

- [x] **Official logo** — `images/logo-veinte-veinte.png`, extracted from the brand's
      source PDF. Native resolution is only 419×146px (the source file has no larger
      version), so it's fine at header/footer size but shouldn't be scaled up much
      beyond that — ask for a higher-res or vector (AI/EPS/SVG) export if it needs to
      go larger anywhere.
- [ ] **Location photos** — `images/optica-el-paso-facade.jpg` and
      `images/optica-el-paso-sign.jpg` referenced in `index.html` but not yet in this
      repo (real phone photos of the location, meant as placeholders until
      professional photography is available). See `images/README.md` for exact
      filenames — drop them in and they appear with no code changes.
- [ ] **Insurance list** — currently generic "most major vision plans" wording;
      swap for a named plan list if/when confirmed.
- [ ] **Domain purchase** — pick and buy a domain, then point it at wherever the
      site ends up hosted.
- [ ] **Hosting / GitHub Pages** — enable Pages on this repo (or pick another static
      host) so the domain has somewhere to point.
- [ ] **Security pass** — see the checklist in the PR/commit notes: repo visibility,
      2FA on the GitHub account, confirm the leaked personal access token from early
      setup was actually revoked, secret scanning enabled.
- [ ] **Page quality score** — once photos + domain are in, run a Lighthouse-style
      audit (performance / accessibility / best practices / SEO) and report the
      score back.

## Structure

```
index.html   — the entire page (HTML/CSS/JS, no dependencies besides Google Fonts)
images/      — logo + location photos referenced by index.html
```
