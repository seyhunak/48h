# 48h Money In — Skill

48-hour sprint to land a first paying customer — `Problem → Buyer → Validation → Solution → Demo → Offer → Payment`.

Portable skill for OpenCode / Codex / Claude Code. Use when you invoke `48h Money In: [DOMAIN] | [LOCATION] | [PRICE]` or `48h Money In: https://...` (URL capture).

## Stack (when you build after "Yes, show me" — generic for any [DOMAIN])

`spec-kit` → Next.js 15 App Router + Tailwind + shadcn/ui + Hallmark Tally (Hum, `npx skills add nutlope/hallmark → hallmark audit → theme`) + full landing (single CTA) + Clean Architecture (`domain/application/infrastructure/presentation`) + Clerk (`ADMIN_EMAIL`, `/app` Clerk-protected) + Convex (real tables, `dev:majestic-wren-98`, `npx convex dev --once`) + SEO (metadata/sitemap/robots/JSON-LD/OG) + Stripe (100 credits — $1,000, $10/credit, free 3 on signup, `Buy → Stripe → /app?credits=added`, keep `stripe listen`) + PDF/CSV + Admin + lucide `ShieldCheck` logo + seed script (`scripts/seed-env.sh`)

- Real `/app` from 0-day: upload → validation → real [DOMAIN] workflow via API → vault (no simulation stub) — e.g. for ZATCA: clearance/reporting; for other domains: replace with your workflow
- Top menu: `logo - App name - Buttons - Logged user + balance` (Admin hidden from public)
- Footer generic: `About · Terms · Privacy · Contact` (200) + `sitemap.xml`/`robots.txt`
- Pre-flight checklist (6): Convex URL no trailing `/`, Convex push, `src/proxy.ts` for Next 16, Clerk `useUser` not `SignedIn`, Stripe `price_...` vs `price_data` + `success_url = req.origin`, Hero single CTA + generic footer

> ZATCA Phase-2 (`https://github.com/seyhunak/zatca-phase2`) is the reference implementation of this skill — same stack, 100 credits $1k free 3, real upload → vault.

## Usage

```
48h Money In: Fintech | Saudi | $1,000 (100 credits $10/credit free 3)
48h Money In: Insurtech | Saudi | $1,000
48h Money In: https://example.com/pricing
```

## Install

```bash
# OpenCode
cp -r 48h-money-in ~/.config/opencode/skills/
# or Codex/Claude
cp -r 48h-money-in ~/.codex/skills/ && cp -r 48h-money-in ~/.claude/skills/
```

## License

MIT — Generic skill, ZATCA as example. Built from iterations on `zatca-phase2/app`.
