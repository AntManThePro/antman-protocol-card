# AntMan Protocol Card

**Source:** `AntMan_Protocol_Card.html` (phone batch, 32,494 bytes, md5 `d3cf99905c4bd312564ace09aea9cc75`) — the one unaudited phone file. Audited Nov 18, 2026.

## What it is

A standalone NEXUS-style achievement/certification card: **The AntMan Protocol — Advanced AI Partnership Mode**. It presents Anthony's method for getting real work out of an AI — 5 protocol steps (challenge deflection, refuse surface responses, create permission for authenticity, recognize breakthroughs, maintain partnership), a 4-level recognition system (Surface Breaker → AntMan Master), achievement indicators, legacy claims, and next steps.

Interactive: level selector, accordion steps, "Open all steps" toggle, and a "Copy the protocol" button (clipboard API with textarea fallback). All content is static text in the page; nothing is saved, nothing is fetched except Google Fonts.

## Audit

- **Banned branding:** 0 hits (godmode2025.net, TwistedGenius).
- **Secrets:** none. No passwords, no tokens, no keys.
- **Network:** 0 fetch/XHR. Only external load is Google Fonts (Orbitron / Rajdhani / Share Tech Mono).
- **JS:** single inline script, passes `node --check`. No localStorage, no demo/seeded data.
- **Changes made (head only):** replaced the `data:,` placeholder favicon with the custom icon set + manifest + theme-color + description. No content changes.

## Verification

Served locally on localhost: all files HTTP 200, title "AntMan Protocol Card" renders. Real-phone test still needed after the live push.

## Publish

- **Target repo:** `antman-protocol-card` (new, public)
- **Push text files:** `index.html`, `manifest.json`, `README.md` (branch `main`)
- **Icons** go via the GitHub web UI into `icons/` (push_files is text-only)
- **Netlify:** import repo, branch main, publish root, no build command, auto-publishing ON, Public. Expected: https://antman-protocol-card.netlify.app/
