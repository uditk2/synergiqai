# SynergiqAI Marketing Page

Single-page, fast, accessible marketing site for **SynergiqAI** built with plain HTML, Tailwind CSS (CDN), and vanilla JS.

## Features

- Responsive, mobile-first layout
- Sticky accessible header + skip link
- Smooth anchor navigation (native CSS `scroll-behavior`)
- ARIA-compliant mobile menu toggle
- WCAG-conscious color contrast & focus states
- Lightweight intersection-based reveal animations (respect `prefers-reduced-motion`)
- SEO + social meta (Open Graph, Twitter, JSON-LD)

## Editing

Open `index.html` and modify sections. Tailwind is pulled via CDN; no build step required.

## Deployment

Any static host (GitHub Pages, Netlify, Vercel, S3, etc.)

Ensure you also host `/favicon.ico` and `/og-image.png` (placeholders referenced in `<head>`).

### Assets

Product logo SVGs included (lightweight placeholders):

- `assets/logos/venturepulse.svg`
- `assets/logos/seerly.svg`
- `assets/logos/apprunner.svg`

Replace with final brand artwork as needed. Keep fallback PNG/WebP optional; currently SVG is referenced for crisp scaling.

### Performance Notes

- Tailwind loaded via CDN with preconnect.
- Images use explicit width/height + `loading="lazy"` + `decoding="async"` to reduce layout shift.
- Minimal JS (no dependencies) ~ few KB.
- Inline critical styles; rest is Tailwind utility from CDN (HTTP/2 cached).

## License

Proprietary – © SynergiqAI.
