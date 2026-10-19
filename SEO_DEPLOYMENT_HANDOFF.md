# SEO patch handoff — Styles of the Nile

## Deployment gate — IMPORTANT
The GitHub main branch currently contains a 5 KB single-file static website with no gallery images, booking page, or mobile collapsible menu. The live ChatGPT Sites site described by the owner has those features. **Do not deploy this repository's index.html over the live site.** First reconcile the live Sites source into this repository or manually port the safe head-only SEO additions from the branch.

## Implemented on this branch
- Canonical URL: https://heru.galorweb.works/
- Robots indexing and image-preview metadata
- Open Graph and Twitter summary metadata
- JSON-LD BarberShop structured data using the business name, address, phone and Instagram URL already present in repository source
- No visual CSS, body content, navigation, or customer copy changed

## Seobility findings requiring live-source access
- Two missing image alt attributes: identify actual images; add descriptive alt only for informative images, alt="" for decorative.
- Apple touch icon: export a 180x180 PNG from the approved barbershop-pole brand asset; add <link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png"> after the file is deployed.
- Repeated <strong> brand phrase: inspect live HTML and reduce only unnecessary semantic emphasis without changing appearance.
- Internal link anchors: inspect actual repeated and long labels; avoid modifying expected navigation labels or breaking booking links.
- UTF-8 HTTP Content-Type response header: configure in actual hosting environment, not solely HTML.
- Backlinks: off-site work requiring legitimate directory/partner citations; no artificial backlinks.
- Subdomain warning: no migration required merely to satisfy Seobility.

## Agent verification before deployment
1. Retrieve actual current live Sites HTML/assets and compare visually and structurally with GitHub.
2. Preserve gallery, booking, mobile/desktop navigation, branding, copy, and all existing functionality.
3. Apply safe metadata changes to current source; confirm canonical matches production URL.
4. Validate JSON-LD and actual business details with owner; check no duplicate conflicting schema.
5. Check every image alt, mobile menu, booking link, favicon/touch icon, response headers, robots and sitemap.
6. Deploy only after source reconciliation and regression testing.
7. Rerun Seobility; record new score and screenshots. Separately check Google Search Console indexing and local visibility; no ranking guarantee.
