# Single Pass — $1 external posture snapshot

**How exposed is your site, really?** One polite automated visit. One categorized report. $1.

## What it does

Single Pass takes a single, clearly-identified automated look at a website (≤5 HTTP requests total) and reports what every visitor's browser can already observe — the security posture your site shows the outside world:

- TLS / certificate posture
- Missing security headers (CSP, HSTS, …)
- Cookie attribute hygiene
- Server version disclosure
- End-of-life dependency fingerprints
- Mixed-content and disclosure-file checks

Findings come back categorized with severity flags (high / medium / low / info) in minutes, delivered to your inbox.

## What it is NOT

Not a security audit, not a penetration test, not a certification. No exploitation, no probing, no fuzzing — nothing beyond a polite read of publicly observable configuration. Reports include no PoCs and no private data.

## How it works

1. **Pay $1** — 1 USDC (Solana) to the address on the live page
2. **Email** the tx signature + your target URL to `singlepasssecure@gmail.com`
3. **Get the report** — categorized findings in minutes. Rate-limited: one snapshot per target per 24h

## For site owners

Opt out any time — send the response header `X-Posture-Snapshot-Optout: 1` or add a robots.txt rule for `SinglePass`; both are honored automatically before any request beyond your homepage.

---

👉 **Live page:** [singlepasssecure-cloud.github.io/singlepass](https://singlepasssecure-cloud.github.io/singlepass/)
