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

- **Testimonials** (Saumya K., Katty M., Maiya R.): need explicit consent from each named consultant.
- **"College Scorecard, IPEDS"** in the data section: only Common Data Sets is partially seeded today; Scorecard + IPEDS integration is on the product roadmap.
- **"Batched monthly refresh"**: not yet wired.
- **Pricing** ($79/$199/Custom): subject to GTM decisions.
- **CCPA compliance**: technical practices align, but customer-facing privacy policy + opt-out flow needs to be documented.
