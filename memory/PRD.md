# MiniDev Landing Page PRD

## Original problem statement
Build an official, production-quality static landing page for the MiniDev Windows beta desktop developer tool. The page must introduce the product, explain its scoped features/specifications/documentation, provide a configurable beta download CTA, and avoid backend, database, authentication, pricing, testimonials, GitHub/source-code references, or unsupported claims.

## Architecture decisions
- React single-page static landing page with reusable data-driven sections and no API calls.
- Download destination is centralized in `frontend/src/config.js` as `DOWNLOAD_URL`.
- Product SEO metadata is defined in `frontend/public/index.html` and reinforced at runtime.
- Responsive CSS uses a dark navy/electric-blue visual system, CSS-only motion, and Lucide icons.

## Implemented
- Sticky responsive navbar with mobile menu and anchor navigation.
- Hero with beta badge, app mockup, download metadata, and two CTAs.
- Introduction, six feature cards, concept comparison, specifications, documentation, database guidance, runtime storage tree, beta notice, requirements, FAQ accordion, download CTA, and footer.
- Accessibility-focused labels, ARIA state on menu/FAQ, focusable controls, and unique `data-testid` coverage.
- SEO title, description, OpenGraph metadata, responsive desktop/tablet/mobile layouts.

## Prioritized backlog
- P0: Replace `GOOGLE_DRIVE_DOWNLOAD_URL` with the final Google Drive installer URL.
- P1: Add a branded favicon and OpenGraph preview image when final brand assets are available.
- P2: Add a short changelog section for future beta releases.