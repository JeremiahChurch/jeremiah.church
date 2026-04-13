# jeremiah.church

Personal site. Astro 5, Tailwind v4, static output. Deployed on Cloudflare Pages.

## Dev

```bash
npm install
npm run dev       # http://localhost:4321
npm run build
npm run preview
```

## Principles

- Zero third-party requests on initial render
- No client JavaScript on first paint
- Strict CSP, HSTS, locked Permissions-Policy (see `public/_headers`)
- `security.txt` at `/.well-known/security.txt` (RFC 9116)

## Deployment

Cloudflare Pages, direct Git integration. Build command `npm run build`,
output `dist/`. Custom domain configured in Cloudflare Pages.
