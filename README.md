# REA — Reverse Engineer Anything

One-command teardown of websites and macOS apps.

    rea <url>       # crawl + fingerprint a website
    rea <path.app>  # inspect a macOS app bundle
    rea --selftest

Output: `~/REA/<slug>/report.md` + `report.html` (dark theme).

**Website mode** extracts: pages crawled, tech stack (Next.js, React, Tailwind, Stripe, Paddle, Firebase, Cloudflare, Sentry, PostHog...), pricing strings, contact emails, signup forms + input fields, download links, meta/OG tags, server headers, page text.

**App mode** extracts: Info.plist (bundle id, version, min macOS, permission usage strings), frameworks (Electron/Swift/Tauri detection), and URLs/API endpoints from the main binary via `strings`.

Stdlib only. Python 3.9+.
