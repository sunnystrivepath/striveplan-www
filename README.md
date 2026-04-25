# striveplan-www

Marketing site for StrivePlan. Lives at https://striveplan.io (eventually). The product app lives in the [`striveplan`](https://github.com/sunnystrivepath/striveplan) repo and runs at https://striveplan.vercel.app.

## What's here

A single-file static site (`index.html`) with inlined CSS + tiny JS for scroll animations. No build step. No framework. Edit the HTML, push to `main`, Vercel redeploys.

## Local preview

```bash
# Any static server works. Easiest:
python3 -m http.server 8080
# or:
npx serve
```

Then open http://localhost:8080.

## Deploy

Vercel auto-deploys `main` on every push. No build configuration needed — Vercel detects `index.html` and serves it as a static site.

## Editing copy

Just edit `index.html`. Search for the section name in the HTML comments (e.g. `<!-- HERO -->`, `<!-- PRICING -->`).

## Things that need separate work before this represents 100% truth

- **"College Scorecard, IPEDS"** in the data section: only Common Data Sets is partially seeded today; Scorecard + IPEDS integration is on the product roadmap.
- **"Batched monthly refresh"**: not yet wired.
- **Pricing** ($79/$199/Custom): subject to GTM decisions.

## Compliance work the site doesn't promise yet (separate roadmap)

- **CCPA compliance**: privacy policy + opt-out / data-deletion request flow. Removed from the page on 2026-04-25 since it isn't yet a documented practice; revisit when ready to make the claim.
- **FERPA-aware practices**: technically aligned (RLS, audit log, soft delete, signed URLs) but not yet documented as a claim on the site.
- **SOC 2**: only mentioned on the Enterprise pricing tier as part of the standard package; actual SOC 2 prep is a separate workstream.
