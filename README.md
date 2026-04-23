# Guidance Funding Website — Static Site Archive

Archive date: **April 23, 2026**

Static multi-page site for Guidance Funding. All files are flat at the repo root; URLs include the `.html` extension (e.g. `/bridge.html`).

## Structure

```
repo-root/
├── index.html           → homepage
├── styles.css           (shared stylesheet)
├── apply.html
├── contact.html
├── bridge.html          (formerly MCA, rebranded)
├── loc.html
├── term.html
├── equipment.html
├── mortgage.html
├── po.html
├── sba.html
├── factoring.html
├── credit-services.html
├── ccp.html
├── bookkeeping.html
├── seo.html
└── payroll.html
```

## Design System

- **Fonts:** Outfit (display headings), DM Sans (body), Montserrat (apply form only)
- **Colors:** `#12948A` (teal), `#0A5D57` (dark teal), `#073F3A` (deep teal), `#F5A623` (amber)
- **Ink:** `#0f1729` / Body text: `#475467`

## Contact info (baked into every page footer)

- Phone: `(213) 522-7765`
- Email: `admin@guidancefunding.com`
- Location: Beverly Hills, CA
- Hours: Monday–Friday, 7am–7pm PST
- License: California Lenders License #60DBO 67237

## Pending items

- **Calendly/booking link** for `contact.html` — "Book a call" button currently `href="#book-link-placeholder"`
- **MyRM redirect** — `apply.html` form submit currently alerts + logs to console. To enable redirect, uncomment near end of `<script>`:
  `// window.location.href = 'https://apply.myrmapp.com/multi-step-apply/lisagl';`

## Edit tips

- Nav and footer are duplicated in every page. To change nav/footer, edit every file.
- `styles.css` affects all pages except `index.html`, which has inline CSS.
- Mobile breakpoints: 1100px, 960px, 560px, 420px. Hamburger appears at 960px.

## Notes

- All internal links use relative paths like `href="bridge.html"`.
- Stylesheet is loaded from the root: `href="styles.css"`.
- Bridge loan product mechanics are the same as a merchant cash advance; only the branding changed. Check with counsel about disclosures if unsure.
