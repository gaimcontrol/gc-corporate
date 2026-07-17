# gc-corporate

> The GaimControl corporate landing at `gaimcontrol.com`.

Positions GaimControl as AI agentic infrastructure for behavioural underwriting. Introduces the three product surfaces (Walkaway, Anna, Holdwell) as one vertically integrated stack. Leads with the recovery-evidence-pack narrative that ties the whole story to a credit outcome.

## Layout

```
gc-corporate/
  index.html         landing page
  assets/
    styles.css       all styles
    logo-mark.svg    GaimControl mark
  README.md
```

## Running locally

Static site. Open `index.html` in a browser, or:

```
npx serve gc-corporate
```

## Deploying

Static Vercel project. Point `gaimcontrol.com` at it.

1. `git init && git add . && git commit -m "gc-corporate v1"`
2. `gh repo create gaimcontrol/gc-corporate --private --source=. --push`
3. Vercel dashboard → New Project → Import `gaimcontrol/gc-corporate`. Framework preset: Other. No build command. Output directory: `.`.
4. Domains → add `gaimcontrol.com` and `www.gaimcontrol.com`. Route 53 → point apex to Vercel (ALIAS to `cname.vercel-dns.com`).
5. When the DNS cuts over, the Taivo redirect drops away naturally.

## Palette

Family with Holdwell and Walkaway.

- Navy grounds: `#0B0F1C`, `#161B2D`, `#20273C`
- Cream ink: `#F5F2EA`
- Honey accent: `#F6C26B` → `#E89537`
- Teal progress: `#5BB088`
- Purple therapy: `#8576C2` (Anna-specific accents only)

## Tone

Quiet, confident, infrastructure. Not consumer, not clinical. Positions GaimControl as the parent of Holdwell + Anna + Walkaway, not as a competitor to any of them.

## Independence disclaimer

Present in the footer. Same text as Walkaway per legal review, extended to also cover Holdwell BaaS + credit-decisioning liability.
