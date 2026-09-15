# 48h Money In — Skill

[![License](https://img.shields.io/github/license/seyhunak/48h-money-in.svg)](./LICENSE)
[![Issues](https://img.shields.io/github/issues/seyhunak/48h-money-in.svg)](https://github.com/seyhunak/48h-money-in/issues)
[![Forks](https://img.shields.io/github/forks/seyhunak/48h-money-in.svg)](https://github.com/seyhunak/48h-money-in/forks)
[![Stars](https://img.shields.io/github/stars/seyhunak/48h-money-in.svg)](https://github.com/seyhunak/48h-money-in/stargazers)

**48-hour sprint to land a first paying customer** — `Problem → Buyer → Validation → Solution → Demo → Offer → Payment`.

Portable skill for OpenCode / Codex / Claude Code. Use when you invoke `48h Money In: [DOMAIN] | [LOCATION] | [PRICE]` or `48h Money In: https://...` (URL capture mode).

## Mission

Find a real, current, expensive problem that companies in a specific domain/location are facing **right now** — one that:
1. Exists today
2. Is painful enough that someone already spends money/time/people dealing with it
3. Has an identifiable buyer with budget
4. Can be solved or materially improved within 48 hours
5. Can be demonstrated without requiring a long implementation
6. Can realistically be sold for the target price range
7. Has a clear reason for the customer to act **now**

**Success = money committed or paid.** Not meetings, not "interest", not GitHub stars.

## Tracks

| Track | Platform | Stack |
|-------|----------|-------|
| **Track A** (default) | Web SaaS | Next.js 15 + Convex + Clerk + Stripe + Hallmark |
| **Track B** | Mobile-only iOS | SwiftUI + Firebase + RevenueCat |

## Stack — Track A (Web SaaS)

`spec-kit` → Next.js 15 App Router + Tailwind + shadcn/ui + **Hallmark** (`npx skills add nutlope/hallmark` → `audit` → pick theme **Tally** (SaaS) / **Hum** (editorial) → `build`) + full landing (single CTA) + **Clean Architecture** (`domain/application/infrastructure/presentation`) + **Clerk** (hosted auth, `ADMIN_EMAIL` admin, `/app` Clerk-protected) + **Convex** (real tables, `dev:majestic-wren-98`, `npx convex dev --once`) + **SEO** (metadata/sitemap/robots/JSON-LD/OG/`llms.txt`) + **Stripe** (100 credits — $1,000, $10/credit, free 3 on signup, `Buy → Stripe → /app?credits=added`, keep `stripe listen`) + PDF/CSV + **Admin** (`/admin`) + lucide `ShieldCheck` logo + **seed script** (`scripts/seed-env.sh`)

- Real `/app` from 0-day: upload → validation → real [DOMAIN] workflow via API → vault (no simulation stub)
- Top menu: `logo - App name - Buttons - Logged user + balance` (Admin hidden from public)
- Footer generic: `About · Terms · Privacy · Contact` (200) + `sitemap.xml`/`robots.txt`
- **Pre-flight checklist (6)**: Convex URL no trailing `/`, Convex push, `src/proxy.ts` for Next 16, Clerk `useUser` not `SignedIn`, Stripe `price_...` vs `price_data` + `success_url = req.origin`, Hero single CTA + generic footer

## Stack — Track B (Mobile-only iOS)

SwiftUI (iOS 17+, 3-tab max, SF Symbols, Dynamic Type) + **Clean MVVM** (Domain/Data/Presentation/Services) + **Firebase** (Auth Apple-first, Firestore real collections, Storage, Functions 2nd gen, FCM, Crashlytics) + **RevenueCat** (`pro` entitlement, `pro_monthly` + `pro_yearly`, 3 free uses → paywall, sandbox StoreKit config, webhook → Firestore entitlements) + `scripts/setup-ios.sh` (asks REVENUECAT/FIREBASE/APPLE keys → `.xcconfig` → resolve deps → reports ready) — working & tested E2E prod-like, real core loop from 0-day, no simulation, distribute via TestFlight internal→external (no App Store review on critical path)

## Usage

```bash
# Standard invocation
48h Money In: Fintech | Saudi | $1,000 (100 credits $10/credit free 3)
48h Money In: Insurtech | Saudi | $1,000
48h Money In: Logistics for SMEs | Berlin, DE | €500–€2k | Web

# URL Opportunity Capture (alternative start)
48h Money In: https://example.com/pricing
48h Money In: https://regulator.gov/new-rule-2026

# Mobile-only shorthand
48h Money In mobile-only: Fitness tracking | UAE | $7.99/mo
48h Money In iOS: Health data export | US | $39/yr
```

## 48-Hour Execution Clock

| Phase | Hours | Output |
|-------|-------|--------|
| **Market Reconnaissance** | 0–2 | 10+ problems, evidence, buyers, economic value |
| **Score & Select** | 2–3 | One problem chosen with scoring |
| **Prospect Research** | 3–5 | 20–50 prospects with contacts & personalization |
| **Offer & Outreach** | 5–8 | Offer, landing/demo page, outreach messages |
| **Validate & Build** | 8–16 | Buying signals → build MVP |
| **Develop MVP** | 16–30 | AI-assisted development |
| **Deploy & Test** | 30–36 | Ship to GitHub (§15), verify E2E |
| **Demo & Close** | 36–48 | Demo, objections, offer, payment |

## Decision Rules

1. **Money before code** — Never build before validating willingness to pay
2. **Sell the problem, not the technology** — Customer buys "70% reduction in manual work", not "AI agent"
3. **Narrow beats broad** — "Automated reconciliation for mid-sized payment companies" > "AI automation for fintech"
4. **Existing pain beats hypothetical demand** — Prefer problems customers already recognize
5. **Urgency matters** — Problem that must be solved this month > problem that can wait 6 months
6. **Build around existing infrastructure** — Integrate before replacing
7. **Human-in-the-loop when appropriate** — For regulated/high-risk workflows
8. **Don't over-engineer** — First customer needs problem solved, not final architecture
9. **One customer is enough** — Objective: get the first person to pay
10. **Kill weak ideas quickly** — If nobody cares, return to market
11. **No automation for outreach** — Manual copy only, no Composio/Gmail/social APIs

## Install

```bash
# OpenCode
cp -r 48h-money-in ~/.config/opencode/skills/
# Codex
cp -r 48h-money-in ~/.codex/skills/
# Claude Code
cp -r 48h-money-in ~/.claude/skills/
```

## Output Format

At every major stage, the skill reports:

- **Current Objective** — What we're trying to achieve
- **Evidence** — What we know from the market
- **Best Opportunity** — The current #1 problem
- **Buyer** — Who can buy
- **Offer** — What we're selling and at what price
- **Next Action** — Single highest-value action
- **Clock** — `HH:MM remaining`

## Obsidian Report + Vault Sync (Mandatory)

At sprint end (and incrementally), generates comprehensive report to `$OBSIDIAN_VAULT/48h/` with:
- Market Research Findings (10+ problems with scoring)
- Selected Problem (description, buyer, economic impact, trigger)
- Prospect List & Contacts (company, buyer, channel, status)
- Solution & Demo (before/after metrics)
- Commercial Outcome (offer, price, close status)

**Vault git sync required after report generation:**
```bash
export OBSIDIAN_VAULT="/Users/seyhunakyurek/Documents/Obsidian/Seyhun Akyurek"
cd "$OBSIDIAN_VAULT"
git config user.name "Seyhun Akyurek"
git config user.email "seyhunakyurek@gmail.com"
git add -A
git commit -m "48h money in: [DOMAIN] [LOCATION] [PRICE] — [outcome]"
git push origin main
```

## Ship to GitHub (Final Build Step)

After MVP built and buying signal received:

1. **Seed + .env setup** — Run `scripts/seed-env.sh` (Track A) or `scripts/setup-ios.sh` (Track B)
2. **Verify locally** — `npm run dev` / `xcodebuild run` with full E2E test
3. **Create GitHub repo + push** — `gh repo create 48h-[domain]-[location] --public --source=. --push`
4. **Add README + DEPLOY.md** — Problem, buyer, solution, tech stack, setup instructions
5. **Deploy** — Vercel (Track A) or TestFlight (Track B)

**Never commit API keys, `.env.local`, `.xcconfig`, or `GoogleService-Info.plist`.**

## License

MIT — Generic skill, [DOMAIN] as example. Built from iterations on `[DOMAIN]-phase2/app`.