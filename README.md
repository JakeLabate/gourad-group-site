# Gourad Group

New website for [gourad.com](https://gourad.com/): Gourad Group, an early stage investor, business incubator
and commercial real estate owner based in Georgetown, Connecticut, founded 1997.

## Structure

Six self-contained static pages. CSS is inlined in each file so every page renders standalone with no build
step and no external stylesheet request.

| File | Purpose |
| --- | --- |
| `index.html` | Home: positioning, service overview, four step process, portfolio index |
| `about.html` | Firm history, what we underwrite, graduated companies |
| `services.html` | Early stage investment, business incubation, commercial real estate |
| `portfolio.html` | Full holdings index plus Connecticut property |
| `spaces.html` | Available commercial space in New Milford and Georgetown, CT |
| `contact.html` | Contact details and a mailto composer |
| `sitemap.xml` | Six URLs |
| `robots.txt` | Allow all, sitemap reference |

## Technical notes

- Canonicals, sitemap and Open Graph URLs point at `https://gourad.com/`, not at this preview host.
- JSON-LD uses a single `@graph` per page with one shared `Organization` node ID reused across the site,
  plus `WebSite`, `WebPage`, `BreadcrumbList`, `Service`, `ItemList` and `Place` nodes where relevant.
- Type: Fraunces, Karla, IBM Plex Mono, loaded from Google Fonts.
- Accessibility: skip link, visible focus rings, semantic landmarks, WCAG AA text contrast, reduced motion
  respected.
- The contact form composes a `mailto:` in the visitor's own mail client. No backend is wired yet.

## Deployment

Flat `.html` URLs. If the live site moves to directory URLs, add 301s from the existing WordPress paths,
including `/gourad_portfolio/` to `/portfolio/` and `/our-process/` to the home page process section.

Built by Jake Labate, SEO Consultant.
