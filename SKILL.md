---
name: 48h-money-in
description: 48-hour sprint to land a first paying customer. Always starts by asking domain(area), location/region, pricing target, and platform (Web SaaS vs mobile-only iOS). Supports Web (Next.js+Convex+Stripe) and mobile-only iOS ideas (SwiftUI+Firebase+Apple IAP via RevenueCat). Use when the user invokes "48h Money In: [DOMAIN] | [LOCATION] | [PRICE RANGE]" or provides a URL to capture domain/target/pricing opportunities, or asks to find/validate/sell a solution to a real expensive problem and close a paying customer within 48 hours. Do not use for long product development or general brainstorming.
---

# Skill: 48h Money In

## Mission

You have **48 hours to generate a paying customer**.

Find a real, current, expensive problem that companies in:

* **Domain:** `[DOMAIN]`
* **Location:** `[LOCATION]`
* **Target company:** `[COMPANY TYPE / SIZE]`
* **Price target:** `[PRICE RANGE]`

are facing **right now**.

You are not looking for interesting ideas.

You are looking for a problem that:

1. Exists today.
2. Is painful enough that someone already spends money, time, or people dealing with it.
3. Has an identifiable buyer.
4. Can be solved or materially improved within 48 hours.
5. Can be demonstrated without requiring a long implementation.
6. Can realistically be sold for `[PRICE RANGE]`.
7. Has a clear reason for the customer to act **now**.

Your objective is:

> **Problem → Buyer → Validation → Solution → Demo → Offer → Payment**

The clock starts immediately.
---

# 0. INTAKE — ASK DOMAIN, LOCATION, PRICING FIRST (MANDATORY)

Do NOT start research until you have these three inputs confirmed.

If the user invoked with `48h Money In: [DOMAIN] | [LOCATION] | [PRICE RANGE] | [Web|iOS]` and domain/location/price are clear (platform defaults to Web if unstated), echo them back in one line and start the clock.

If any are missing, vague, or only inferable — ASK before researching. Use the `question` tool (or plain questions if unavailable) with these exact questions:

1. **Domain (area)?** — What industry / problem area to hunt in?
   - Example answers: `logistics for SMEs`, `dental clinics`, `e-commerce fulfillment`, `construction compliance`
   - Accept broad + narrow. If broad, propose a narrow slice after answer.

2. **Location / region?** — Where are the customers?
   - Example answers: `Berlin, DE`, `DACH`, `UAE`, `US remote`, `global / English-speaking`
   - Needed for regulations, pricing comps, language, outreach channels, time zones.

3. **Pricing target?** — What should one customer pay?
   - Example answers: `$500 one-time`, `$1k setup + $200/mo`, `$3k–$5k pilot`, `€500–€2k`, `TBD — propose 3 anchors`
   - If user says TBD / don't know, propose 3 anchors based on domain + location and let them pick one.
   - For mobile-only: answer as IAP subscription target, e.g. `$4.99–$9.99/mo or $39–$79/yr`.

4. **Platform?** — Web SaaS or mobile-only iOS?
   - Options: `Web SaaS (Next.js + Convex + Stripe)` (default) / `Mobile-only iOS (SwiftUI + Firebase + RevenueCat)`
   - Ask this always — do not infer from domain alone. If user says `mobile`, `iOS`, `iPhone`, `App Store`, route to Track B (§5 Track B).
   - If invocation already states platform (e.g. `mobile-only`, `iOS`, `SwiftUI`), echo it and skip asking.

Rules:
- Ask all missing inputs in ONE batch, not one-by-one.
- Never silently infer location or pricing — a wrong guess wastes the 48h.
- Company type/size is optional bonus (infer from domain unless B2B enterprise — then confirm buyer).
- Platform routing: `Web` → §5 Track A, `Mobile-only iOS` → §5 Track B. State the chosen track explicitly.
- Once answered, restate as: `48h Money In: [DOMAIN] | [LOCATION] | [PRICE] | [Web|iOS] — clock started` and proceed to §1.
- URL mode (§14): still run URL capture first, then fill gaps by asking only what's still missing.

---

# 1. FIND THE MONEY

Research the target market aggressively.

Use **Google, Exa, Tavily, and other search engines and job boards** to find evidence of real problems.

**Do not visit LinkedIn at all.**

Look for evidence of real problems through:

* Recent company announcements
* Job postings
* Customer complaints
* Industry forums
* Reddit
* X discussions
* Product reviews
* Regulatory changes
* Government announcements
* Industry reports
* Tender/RFP documents
* Company documentation
* Support pages
* Engineering blogs
* Security/compliance requirements
* Operational bottlenecks
* Repetitive manual processes
* Recently introduced regulations
* New technology adoption
* Hiring patterns
* Recent layoffs/restructuring
* Publicly visible workflow problems

Prioritize problems with **financial consequences**.

For every candidate problem, estimate:

* Who experiences it?
* How frequently?
* What does it cost?
* What happens if they don't fix it?
* Who owns the problem?
* Who has budget?
* What are they currently using?
* Why isn't the existing solution good enough?
* Why would they buy from me instead of doing nothing?
* Why can I solve it in 48 hours?

Do not settle for generic problems such as:

> "Companies need AI automation."

Instead find:

> "Operations teams at X-type companies spend 15 hours/week manually reconciling Y because their existing system doesn't handle Z."

---

# 2. SCORE THE PROBLEMS

Generate at least **10 potential problems**.

Score each from 1–10:

| Dimension         | Question                                   |
| ----------------- | ------------------------------------------ |
| Pain              | How painful is this?                       |
| Frequency         | How often does it happen?                  |
| Financial Impact  | Does it cost real money?                   |
| Urgency           | Why solve it now?                          |
| Buyer Clarity     | Can I identify the buyer?                  |
| Budget            | Is there likely budget?                    |
| Accessibility     | Can I reach the buyer?                     |
| 48h Feasibility   | Can I build a credible solution quickly?   |
| Differentiation   | Can I offer something meaningfully better? |
| Sales Probability | Can this realistically close quickly?      |

Calculate an overall score.

**Do not choose the most technically interesting problem.**

Choose the problem with the highest probability of producing money within 48 hours.

---

# 3. SELECT ONE PROBLEM

Once the evidence is sufficient, commit to **ONE** problem.

Produce:

### Problem

One sentence describing the painful problem.

### Buyer

The exact person who can approve the purchase.

Examples:

* COO
* Head of Operations
* CFO
* Head of Compliance
* CTO
* Head of Risk
* Head of Customer Support
* Founder

### Existing workaround

What they currently do.

### Cost of the problem

Estimate the economic impact.

### Trigger

What makes this problem urgent now?

### Solution

Describe the smallest solution that creates measurable value.

### 48h promise

Explain what can realistically be delivered in 48 hours.

### Commercial offer

Define:

* Setup price
* Optional recurring price
* Scope
* Deliverables
* Timeline
* Customer responsibilities
* Success criteria

---

# 4. VALIDATE BEFORE BUILDING

Do **not** spend 30 hours building something nobody wants.

Validate the problem first.

Find real companies that appear to have the problem.

Create a short outreach message that communicates:

> I noticed X.
>
> Companies like yours appear to be dealing with Y.
>
> I built a small solution that can reduce/eliminate Z.
>
> I can have it running for you within 48 hours.
>
> Would it be useful if I showed you a 10-minute demo?

Contact as many relevant prospects as realistically possible.

Prioritize:

1. Warm contacts
2. Existing network
3. Email (manual send by the user)
4. X (manual post/DM by the user)
5. Industry communities
6. Direct company contact
7. Other relevant channels

### Outreach execution rules — NO automation (mandatory)

- Do **NOT** use Composio, Gmail tools, mailbox APIs, auto-senders, schedulers, or any email-sending integration — no `COMPOSIO_*`, no `GMAIL_*`, no draft creation, no sends.
- Do **NOT** touch the user's mailbox, contacts, or social accounts in any way.
- Provide ready-to-paste outreach copy (subject + body + personalization slots like `[Name]`, `[Company]`) for the user to send manually. Max 3 messages per batch unless the user explicitly raises the cap.
- Same for X/DMs/communities: ready-to-paste text only, never auto-post.
- Log outreach as "drafted for manual send", never as "sent", and always report the exact copy in chat + Obsidian report.

The goal is not engagement.

The goal is:

> **"Yes, show me."**

---

# 5. BUILD ONLY AFTER BUYING SIGNAL

If the problem is validated, build the smallest possible solution.

You may use:

* Claude Code
* OpenCode
* Kilo Code
* Cursor
* GitHub
* Supabase
* Vercel
* Cloudflare
* APIs
* LLMs
* Automation platforms
* Existing SaaS
* Open-source software

Use AI aggressively.

The objective is not to demonstrate engineering ability.

The objective is to create **customer value**.

Prefer:

> Working ugly prototype

over:

> Beautiful unfinished product.

Build only what is required to demonstrate the promised outcome.

### Track A — Web SaaS (default) — Generate via spec-kit (GitHub)

When you do build, **suggest generating the app with [github/spec-kit](https://github.com/github/spec-kit)** — spec-driven, white-label ready, 1-day capable. After building, run §15 SHIP TO GITHUB to seed, set up .envs, and push to a GitHub repo (created if needed).

- **Spec first:** `/spec` writes the 48h fix-pack spec (problem → buyer → scope → success criteria) before code — matches §3 SELECT ONE.
- **Frontend:** **Next.js 15 App Router + Tailwind + shadcn/ui + full landing page** — marketing landing (hero with **single primary CTA** `Upload 10 invoices — see cleared →` only, no `$3k Fix-Pack` hero button, problem → before/after, pricing 100 credits — $1,000 ($10/credit), social proof, FAQ) + app — fast to brand (logo/colors/subdomain, single `ShieldCheck` logo + App name, no extra icons), responsive, Vercel-deployable in 1 click. **Use [Hallmark](https://www.usehallmark.com) ([github](https://github.com/nutlope/hallmark))** — install `npx skills add nutlope/hallmark` (auto-detected: Claude Code `~/.claude/skills/hallmark/`, Codex `~/.codex/skills/hallmark/`, Cursor `.cursor/rules/hallmark.mdc`; then just ask for UI — hallmark attaches via `hallmark.observe()`). 48h workflow: `hallmark audit` current page (ranked punch list, **no edits**) → pick theme (default **Tally** for SaaS fix-pack, **Hum** for editorial; 20 themes, press T to preview) → `hallmark build` with theme (macrostructure → theme → enrichment; stamped, slop-tested; refuses repeating last 3 macrostructures) → apply tokens to landing + `/app`. Extra verbs: `hallmark study <URL|screenshot>` → DNA card (`lock the DNA` → portable `design.md`, never copies pixels); `hallmark redesign` keeps content/brand, changes bones. Obey 8 foundations (display+body font pair, never Inter-everywhere; OKLCH 1 anchor hue, accent <5%; spacing multiples of 4; asymmetric biased layout; exponential ease-out + reduced-motion; distinct voice; display/body/label hierarchy) and avoid the 5 slop tells audit flags (purple-gradient hero → solid + single accent; Inter-as-display; centred-everything; icon-tile feature cards; generic AI nav). **Codebase must follow Clean Architecture** — `src/domain` (entities/use-cases, no framework), `src/application` (services, ports), `src/infrastructure` (Convex/Clerk/Stripe/PDF adapters), `src/presentation` (Next.js app routes + shadcn components) → dependency rule points inward, Hallmark tokens live only in presentation. **Use proper logo from icon library** — `lucide-react` `ShieldCheck` single + wordmark, token-colored. **Top menu (N5 pill → N1b for Hum) must show** `logo - App name - Buttons (App, Admin if admin) - Logged user + balance (if logged)` — Clerk `<UserButton>` / `useUser()` avatar + email + credits badge + **Buy Credits → Stripe Checkout** → redirect back to `/app` (success_url=`/app?credits=added`), keep `stripe listen` open; also show **Logout/Login**. **Admin link must NOT appear in public** — only visible to admin user. **Footer must be generic** — `About`, `Terms`, `Privacy`, `Contact`, `Sitemap`, `Robots` (all 200, not 404), no `White-label experiment — 1 customer · 1 day` text.
- **Auth:** **Clerk** — hosted auth (sign-in/up, orgs), webhook → Convex `users`, **admin user for me** (seeded via `ADMIN_EMAIL` env, role=admin). No custom auth.
- **Backend:** **Convex** — real tables (no dummy data), schema in `convex/schema.ts` (tenants, users, invoices, submissions, credits, vault), file storage for XML/PDF, realtime queries. **Just put API keys in `.env.local` and it is ready — max 1 minute setup** (`NEXT_PUBLIC_CONVEX_URL`, `CLERK_*`, `STRIPE_*`). **Push live:** after seed, run `npx convex codegen` + `npx convex dev --once --typecheck disable` (dev at `dev:majestic-wren-98`, prod via `npx convex deploy --yes`) — ensure DB, schema, indexes, and functions (`credits:getBalance/getOrCreate/consume/addCredits`) are built and deployed; verify with `npx convex run credits:getOrCreate '{"clerkId":"test123"}'`. No seed stubs.
- **SEO (when creating app):** **Always include SEO** — Next.js Metadata API (title/description/canonical/OG/Twitter), `sitemap.ts`, `robots.ts`, `llms.txt`, JSON-LD (Organization + Product + FAQ), OG image (1200x630), `next-sitemap` or `next-seo`, and keyword-ready blog stub (`/blog`). Hallmark theme must not break SEO (semantic headings, alt text, meta).
- **Billing:** **Stripe — 1 fixed package, credit-based usage** — **100 credits — $1,000 ($10/credit)**, credits decrement per use (1 credit per invoice), **free 3 on signup**, customer portal + webhook (`stripe listen --forward-to localhost:3000/api/webhooks/stripe` kept open) → Convex `credits`/`subscriptions`. **Buy Credits in top menu goes to Stripe Checkout (100 credits, $10/credit) and on success redirects back to `/app` — webhook must update Convex DB (`credits` +100) and UI must reflect new balance immediately (no manual refresh).** No tier sprawl. **Pilot — $1,000, Enterprise — $1,000 + $2,000/mo**.
- **Docs:** **PDF + CSV generation** — server-side PDF (report, vault export) + CSV exports (queue, vault) — tested with real domain field names (replace with your [DOMAIN] fields).
- **Ops:** **Admin panel** — `/admin` (Clerk protected, `role=admin` from Convex) — manage customers, view submissions, trigger re-runs, see Stripe + credits logs, toggle per-tenant branding. Admin is your `ADMIN_EMAIL`.
- **Ready to use (non-negotiable):** **Working & tested E2E before handoff — prod-like, no dummy checks, real implementation from 0-day.** After generation, `put keys in .env.local → max 1m setup → npm run dev →` announce and users can **register/login (Clerk) → buy credits (100 credits — $1,000, $10/credit, free 3 on signup) → start using (1 credit per invoice) → vault/PDF/CSV** with no extra dev — **customer invited on day 0 can use the app immediately, no simulation stub.** **`/app` must be Clerk-protected** (`src/proxy.ts` clerkMiddleware + `createRouteMatcher(['/app(.*)','/admin(.*)'])` → `auth.protect()`) **and must do login check + credits check + UI works as designed** — unauthed redirects to `/sign-in`, no credits shows “buy 100”, with credits shows **real workbench (upload → validation → real [DOMAIN] workflow via API → vault)** fully interactive, Hallmark-themed, responsive at 320/375/414/768. **No simulation — `/app` is the real implementation of the solution for your [DOMAIN] (not stub), customer can invite and use from 0-day.** **Stripe sandbox buy must update DB and UI: `checkout.session.completed` → Convex `credits` +100 via webhook, and `/app?credits=added` must refetch and show new balance without manual refresh.** **If seed ran before and `.env.local` is already valid, `npm run dev` just validates (checks Convex/Clerk/Stripe connectivity, no re-prompt).** Require `npm run build` + `npm run test:e2e` (real Clerk sign-up, real Stripe test checkout → webhook → Convex +100 → UI badge updates, real PDF download, login/credits UI assertions, real clearance call) passing — **no `if (!key) use dummy` branches, no `simulateClearance` stub in prod path.** Then run §15 SHIP TO GITHUB to create/push the repo and deploy to Vercel.
- **Seed script (after generation):** **Create `scripts/seed-env.sh` (or `scripts/setup.ts`) that asks you for API keys** — `NEXT_PUBLIC_CONVEX_URL`, `CONVEX_DEPLOYMENT`, `NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY`, `CLERK_SECRET_KEY`, `CLERK_WEBHOOK_SECRET`, `STRIPE_SECRET_KEY`, `NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY`, `STRIPE_WEBHOOK_SECRET`, `STRIPE_PRICE_CREDITS`, `NEXT_PUBLIC_SITE_URL`, `ADMIN_EMAIL` — **you paste them, it writes `.env.local` and `.env.production` (or Vercel env), runs `npx convex codegen` + `npx convex dev --once --typecheck disable` (or `npx convex deploy --yes` for prod) + `npm run build` check, verifies `npx convex run credits:getOrCreate` (free 3), then reports `✓ ready — register/login → buy credits (100 credits $1k, $10/credit, free 3) → start using` confirmation. On subsequent `npm run dev`, it only validates existing `.env.local` instead of re-asking.**
- **Preview:** **Cloudflare Tunnel (free)** — creates a secure, encrypted tunnel from your local machine to Cloudflare’s edge. Install `cloudflared` (`brew install cloudflared` / `npm i -g cloudflared`), then `cloudflared tunnel --url http://localhost:3000` while `npm run dev` is running to share a public `https://*.trycloudflare.com` link instantly (no deploy) for customer demo before Vercel.
- **Pre-flight checklist (before `npm run dev` — prevents the 15 fixes above):**
  1. **Convex URL:** `NEXT_PUBLIC_CONVEX_URL` has **no trailing `/`** (`https://xxx.convex.cloud` not `.../`), `src/components/ConvexClientProvider.tsx` does `raw.replace(/\/+$/,'')`; otherwise `wss://...//api/...` → `1006`.
  2. **Convex push:** `CONVEX_DEPLOYMENT=dev:<name>` matches URL (e.g. `dev:majestic-wren-98`), then `npx convex codegen` + `npx convex dev --once --typecheck disable` (dev) or `npx convex deploy --yes` (prod) — verify `npx convex run credits:getOrCreate '{"clerkId":"test123"}'` returns `balance:3` (free 3); if `Could not find public function`, re-push.
  3. **Middleware location:** Next 16 + `src/` → file must be `src/proxy.ts` (not `middleware.ts` or root) — `clerkMiddleware` + `createRouteMatcher(['/app(.*)','/admin(.*)'])` → `auth.protect()`; both files → error `Both middleware and proxy file are detected`.
  4. **Clerk UI:** never `SignedIn`/`SignedOut` (removed in Core 3) and no `UserButton afterSignOutUrl` — use `useUser()` + `isLoaded ? !user ? Login/Sign up : UserButton + credits + Buy`; `src/middleware` deprecation `createRouteMatcher` → keep but note.
  5. **Stripe price:** `STRIPE_PRICE_CREDITS` may be `price_...` or `100` — `src/app/api/checkout/route.ts` must branch `isPriceId ? {price} : {price_data:{currency:"usd", product:"100 credits @ $10/credit", unit_amount:100000}}` ($1,000 for 100 → $10/credit); `success_url` must be `new URL(req.url).origin + "/app?credits=added"` (not `NEXT_PUBLIC_SITE_URL` prod on localhost). Webhook `src/app/api/webhooks/stripe/route.ts` must skip verification if `STRIPE_WEBHOOK_SECRET` is `...` placeholder, otherwise `whsec_...` from `stripe listen --forward-to localhost:3000/api/webhooks/stripe` must be kept open, and `/app?credits=added` must refetch Convex `getBalance` via realtime (no manual refresh).
  6. **Hero/Footer:** Hero has **single CTA** (`Upload 10 invoices — see cleared →` only, no `$3k Fix-Pack` button) and footer is **generic** (`About`, `Terms`, `Privacy`, `Contact`, `Sitemap`, `Robots` all 200) — no `White-label experiment — 1 customer · 1 day` text; create `src/app/about|terms|privacy|contact/page.tsx` + `sitemap.ts` includes them, otherwise 404.

> Prompt hint: `spec-kit: Next.js 15 App Router + Tailwind + shadcn/ui + Hallmark (audit → Tally/Hum theme → build; foundations: font-pair, OKLCH 1-hue, asymmetric, no slop) + full landing + Clean Architecture (domain/application/infrastructure/presentation) + Clerk (admin user, /app Clerk-protected with login + credits check, top menu logo - App name - Buttons - Logged user + balance) + Convex (real tables, no dummy, 1m setup, prod-like, push live via convex dev --once + deploy) + SEO (metadata/sitemap/robots/JSON-LD/OG/llms.txt) + Stripe (100 credits — $1,000, $10/credit, free 3 on signup, top-menu Buy Credits → Stripe → /app?credits=added, keep stripe listen) + PDF/CSV + /admin + proper logo (lucide ShieldCheck) + seed script (asks for CONVEX/CLERK/STRIPE keys → writes .env.local + prod → codegen + dev --once + build → reports ready, 100 credits $1k) — working & tested E2E prod-like, real implementation (100 credits $10/credit, /app real [DOMAIN] workflow from 0-day, no simulation), preview via Cloudflare Tunnel then deploy to Vercel.`

This keeps §5 Track A narrow (one fix-pack schema, one customer tenant) while leaving monetization + audit trails production-ready.

### Track B — Mobile-only iOS (SwiftUI + Firebase + RevenueCat)

Use when §0 Platform = `Mobile-only iOS`, or the idea only makes sense as an iPhone app (camera, push, widgets, HealthKit, offline-first, App Store distribution). Do NOT force the Web SaaS stack onto a mobile-only idea.

When you do build, **suggest generating the app spec-first** (same `/spec` discipline as Track A: problem → buyer → scope → success criteria → paywall), then build native:

- **Spec first:** `/spec` writes the 48h mobile fix-pack spec (problem → user → single core loop → paywall → success metric) before code — matches §3 SELECT ONE. Scope to ONE core loop + paywall, nothing else.
- **Frontend:** **SwiftUI (iOS 17+, Swift 5.9+, Xcode 15+)** — single app target, `TabView` max 3 tabs (Core loop + History/Vault + Settings), native NavigationStack, SF Symbols only (no custom icon sprawl), Dynamic Type + VoiceOver + reduced-motion support, light/dark ready. No UIKit unless a wrapped component forces it.
- **Architecture:** Clean MVVM — `Domain` (entities/use-cases, no Firebase import), `Data` (Firebase repositories), `Presentation` (SwiftUI Views + ViewModels, `@MainActor`), `Services` (RevenueCat, push, analytics protocols). Dependency rule points inward. No business logic in Views.
- **Auth + Backend:** **Firebase** — Firebase Auth (Sign in with Apple mandatory if any third-party sign-in; anonymous → upgrade path allowed for 48h demo), Cloud Firestore (real collections: `users`, `workspaces`, `items/submissions`, `entitlements`, `events` — no dummy data), Firebase Storage (images/PDFs), Cloud Functions (Swift/TS, 2nd gen) for webhooks + server-side validation, FCM push, Crashlytics + Analytics from day 0. **Just put `GoogleService-Info.plist` + `.xcconfig` keys and it is ready — max 5 minute setup.** Security Rules locked-down (owner-only read/write, `request.auth != null`), Firestore indexes committed (`firestore.indexes.json`), verified with emulator (`firebase emulators:start`) before prod push.
- **Billing (non-negotiable):** **Apple In-App Purchase, subscription managed with RevenueCat** — NO Stripe, NO custom billing, NO web checkout bypass (App Store rule). Setup: 1 monthly + 1 annual product in App Store Connect (e.g. `pro_monthly $7.99/mo`, `pro_yearly $59.99/yr` — adjust to §0 pricing target), mirrored in RevenueCat (`pro` entitlement), `Purchases.configure(apiKey)` + `login(appUserID)` on auth, paywall triggered after 3 free uses (mirror of Track A free-3 pattern), restore-purchase in Settings, sandbox tested with StoreKit Configuration file + RevenueCat sandbox. Webhook: RevenueCat → Cloud Function → Firestore `entitlements` (never trust client-side `isPro` alone). Gating: no entitlement → paywall sheet, with entitlement → full core loop.
- **Seed script (after generation):** Create `scripts/setup-ios.sh` (or `scripts/setup.rb`) that asks for `REVENUECAT_IOS_API_KEY`, `FIREBASE_PROJECT_ID`, `APPLE_TEAM_ID`, `BUNDLE_ID`, product IDs (`PRO_MONTHLY`, `PRO_YEARLY`), then writes `.xcconfig` + validates `GoogleService-Info.plist` bundle match + runs `xcodebuild -resolvePackageDependencies` + `firebase use --add` check, then reports `✓ ready — run → sign in (Apple) → 3 free uses → paywall (RevenueCat sandbox) → core loop → history/share` confirmation. On subsequent runs it only validates, never re-asks.
- **Preview + distribution (48h-safe):** NO App Store review on the critical path — demo via local build + Screen Recording, then **TestFlight internal (1–5 testers, available in minutes) → TestFlight external (up to 10k, no full review for first external build review ~ hours)**. Customer invited on day 0 can use the app immediately via TestFlight, no review stub. Archive with `xcodebuild archive` + upload via Transporter/`xcrun altool`; version bump `CFBundleShortVersionString` per upload.
- **Ready to use (non-negotiable):** **Working & tested E2E before handoff — prod-like, no dummy checks, real implementation from 0-day.** After generation, `put keys in .xcconfig → run on simulator/device →` announce and users can **sign in (Apple) → 3 free uses → paywall (RevenueCat) → subscribe (sandbox) → core loop → history/share/export** with no extra dev. **No `isPro = true` debug bypass in release path, no `simulatePurchase` stub in prod path.** Then run §15 SHIP TO GITHUB to create/push the repo and deploy to TestFlight. Require `xcodebuild test` (real Auth sign-in, real RevenueCat sandbox purchase → Firestore `entitlements/pro=true` → paywall unlocks, real export/share) passing.
- **Pre-flight checklist (before `xcodebuild run`):**
  1. **Bundle match:** `BUNDLE_ID` in Xcode == App Store Connect == `GoogleService-Info.plist` `BUNDLE_ID` == RevenueCat app config; otherwise Auth/push/IAP all fail silently.
  2. **Sign in with Apple:** capability ON + App ID configured; Firebase Auth Apple provider enabled with Services ID + key.
  3. **RevenueCat products:** `pro_monthly`/`pro_yearly` exist in App Store Connect (Ready to Submit minimum) AND linked to `pro` entitlement in RevenueCat; StoreKit config file includes both for local testing.
  4. **Firestore rules:** `firebase deploy --only firestore:rules` pushed; emulator test passes for owner-only + entitlement-gated reads.
  5. **Paywall copy:** price + trial/terms + `Restore Purchases` + Privacy/Terms links (App Store rejection prevention); no `Subscribe` button that does nothing.

> Prompt hint: `mobile fix-pack iOS: SwiftUI (iOS 17+, 3-tab max, SF Symbols, Dynamic Type) + Clean MVVM (Domain/Data/Presentation/Services) + Firebase (Auth Apple-first, Firestore real collections, Storage, Functions 2nd gen, FCM, Crashlytics) + RevenueCat (pro entitlement, pro_monthly + pro_yearly, 3 free uses → paywall, sandbox StoreKit config, webhook → Firestore entitlements) + scripts/setup-ios.sh (asks REVENUECAT/FIREBASE/APPLE keys → .xcconfig → resolve deps → reports ready) — working & tested E2E prod-like, real core loop from 0-day, no simulation, distribute via TestFlight internal→external (no App Store review on critical path).`

Track selection rule: §0 Platform decides. Web → Track A only. iOS mobile-only → Track B only. Never mix Stripe into iOS or RevenueCat into Web. Landing page for Track B = App Store listing assets (subtitle, screenshots plan, paywall copy) + optional one-page web teaser, not a full Next.js site.

---

# 6. CUSTOMER-SPECIFIC DELIVERY

Do not build a generic product if a customer-specific solution can close faster.

If necessary:

* Configure the customer's workflow.
* Import sample data.
* Connect their existing tools.
* Build a custom dashboard.
* Create an automation.
* Build an internal tool.
* Add an AI agent.
* Create an API.
* Create a report generator.
* Automate a repetitive process.
* Add monitoring.
* Add authentication.
* Add basic auditability.
* Document the workflow.

Make the solution feel like:

> **"This was built for our problem."**

---

# 7. DEMO

Create a **5–10 minute demo**.

The demo must follow:

### Before

Show the current painful workflow.

### Intervention

Show the solution.

### After

Show the measurable improvement.

For example:

> Before: 3 hours of manual work.

> After: 12 minutes.

or:

> Before: 400 documents manually reviewed.

> After: AI processes them and flags the 17 requiring human attention.

or:

> Before: customer requests wait 24 hours.

> After: automatically classified and routed in seconds.

Never spend the demo explaining architecture unless the buyer asks.

Sell the outcome.

---

# 8. MAKE THE OFFER

Do not ask:

> "What do you think?"

Ask for the sale.

Present a concrete offer.

Example:

> I'll deploy this for your team within 48 hours.
>
> Initial implementation: `[PRICE]`
>
> Includes:
>
> * X
> * Y
> * Z
> * 48h deployment
> * 14 days of support
>
> If it doesn't deliver `[SUCCESS CRITERIA]`, we'll stop and reassess.

Adjust the commercial structure to reduce perceived risk.

Possible models:

### Fixed implementation

`$X – $Y`

### Paid pilot

`$X`

### Setup + subscription

`$X setup + $Y/month`

### Outcome-based

Lower upfront cost + payment tied to measurable result.

Do not automatically discount.

If the problem is worth $100k/year to the customer, a $5k implementation may be cheap.

---

# 9. CLOSE

Handle objections directly.

### "We need to think about it."

Ask:

> "What specifically do you need to evaluate before deciding?"

### "It's too expensive."

Ask:

> "Compared with the cost of continuing the current process, or compared with another solution?"

### "We already have a solution."

Ask:

> "What does your current solution handle well, and where does it still require manual work?"

### "We need procurement."

Find the smallest legitimate entry point:

> paid pilot / proof of value / departmental deployment / professional services engagement.

Do not attempt to bypass procurement, security, compliance, or legal requirements.

---

# 10. 48-HOUR EXECUTION CLOCK

## Hour 0–2

Market reconnaissance.

Output:

* 10+ problems
* Evidence
* Potential buyers
* Estimated economic value

Begin building the Obsidian report with all findings. Save incrementally to `$OBSIDIAN_VAULT` and run an **incremental vault sync** (`git add -A && git commit && git push`) so work is never lost.

## Hour 2–3

Score problems.

Choose **ONE**.

## Hour 3–5

Research 20–50 potential prospects.

Identify:

* Company
* Buyer
* Evidence of problem
* Contact channel
* Personalization angle

Log all findings to the Obsidian report incrementally.

## Hour 5–8

Create:

* Offer
* Landing/demo page
* Outreach message
* Demo concept

Start outreach.

## Hour 8–16

Talk to prospects.

Validate.

Build only what receives buying signal.

## Hour 16–30

Develop MVP.

Use AI coding agents aggressively.

Ship continuously.

## Hour 30–36

Deploy — run §15 SHIP TO GITHUB (seeds + .env setup + repo push).

Test.

Create customer-specific demo.

## Hour 36–42

Demo.

Collect objections.

Fix critical issues.

Present commercial offer.

## Hour 42–48

Close.

Send:

* Proposal
* Scope
* Price
* Payment instructions
* Implementation timeline

Generate the final Obsidian report with all findings, problems, and contacts, then **immediately run the Vault git sync** from §13 (commit + push to `seyhunak/obsidian-vault:main`), and verify the solution repo is pushed to GitHub per §15 (commit + push, create repo if needed).

**Success = money committed or paid.**

Not:

* GitHub stars
* Website traffic
* Prototype completion
* "Interesting idea"
* Meetings booked
* People saying "cool"

---

# 11. DECISION RULES

Follow these rules throughout the sprint.

### Rule 1 — Money before code

Never spend significant development time before validating willingness to pay.

### Rule 2 — Sell the problem, not the technology

The customer doesn't buy:

> "An AI agent."

They buy:

> "A 70% reduction in manual compliance review."

### Rule 3 — Narrow beats broad

Bad:

> AI automation platform for fintech.

Good:

> Automated reconciliation exception handling for mid-sized payment companies.

### Rule 4 — Existing pain beats hypothetical demand

Prefer problems customers already recognize.

### Rule 5 — Urgency matters

A problem that is painful but can wait six months is inferior to a problem that must be solved this month.

### Rule 6 — Build around existing infrastructure

Integrate before replacing.

### Rule 7 — Human-in-the-loop when appropriate

For regulated or high-risk workflows, automate the work around the decision rather than pretending humans aren't needed.

### Rule 8 — Don't over-engineer

The first customer doesn't need your final architecture.

They need the problem solved.

### Rule 9 — One customer is enough

The objective is not to build a unicorn in 48 hours.

The objective is:

> **Get the first person to pay.**

### Rule 10 — Kill weak ideas quickly

If nobody cares, stop building.

Return to the market.

### Rule 11 — No Composio / mailbox / social automation

Never use Composio, Gmail, mailbox APIs, or social-posting tools in this sprint — no sends, no drafts, no mailbox reads for outreach. Outreach is manual copy the user sends; the skill only drafts text and logs it.

---

# 12. OUTPUT FORMAT

At every major stage, report:

## Current Objective

What we're trying to achieve.

## Evidence

What we know from the market.

## Best Opportunity

The current #1 problem.

## Buyer

Who can buy.

## Offer

What we're selling and at what price.

## Next Action

The single highest-value action to take next.

## Clock

`HH:MM remaining`

---

# 13. OBSIDIAN REPORT + VAULT SYNC (MANDATORY)

At the end of the sprint — and incrementally throughout — generate a comprehensive report and save it to the Obsidian vault. The report must contain:

### Market Research Findings

* All problems identified (10+ candidates with evidence)
* Scoring results for each problem
* Market signals and sources used

### Selected Problem

* The chosen problem description
* Buyer profile and rationale
* Economic impact estimate
* Trigger/urgency

### Prospect List & Contacts

* All potential prospects researched (company, buyer name/role, contact channel, personalization angle)
* Outreach messages sent and responses received
* Status of each prospect (contacted, responded, in demo, closed)

### Solution & Demo

* Solution description
* Demo key metrics (before/after)

### Commercial Outcome

* Offer presented
* Price and terms
* Close status (paid, committed, or lost)

Save the report as a dated note in the Obsidian vault (e.g., `48h-money-in-2026-09-01.md`) and also under `48h/` if the sprint is domain-specific (e.g., `48h/48h-money-in-YYYY-MM-DD-domain.md`). Link it from the relevant project or daily note. Use the `obsidian-wiki-ingest` or `wiki-capture` skill if available.

### Vault git sync — required after report generation

The Obsidian vault at `~/Documents/Obsidian/Seyhun Akyurek` is a git repo synced to `seyhunak/obsidian-vault` (`main`). **Whenever the vault gains or edits markdown files, you MUST commit and push.**

After writing the report (and at each major stage if files were created), run:

```bash
export OBSIDIAN_VAULT="/Users/seyhunakyurek/Documents/Obsidian/Seyhun Akyurek"
cd "$OBSIDIAN_VAULT"

# verify identity
git config user.name "Seyhun Akyurek"
git config user.email "seyhunakyurek@gmail.com"

# stage — respect .gitignore (never force-add .smart-env, .opencode, .ok, .codex, .claude, .agents, .cursor, node_modules, .DS_Store, .obsidian/workspace*.json)
git add -A
# unstage sensitive/local-only if accidentally staged
git restore --staged .env 2>/dev/null; git restore --staged "*.bak" 2>/dev/null

git status --short
git diff --cached --stat

# meaningful commit message — include DOMAIN, LOCATION, price, and outcome
git commit -m "48h money in: [DOMAIN] [LOCATION] [PRICE RANGE] — [1-line outcome / close status]"

git push origin main
```

Rules:
- Do NOT skip the push — the vault's GitHub repo is the source of truth.
- Do NOT force-add ignored paths.
- If `git push` fails (e.g., behind remote), `git pull --rebase origin main` then retry.
- During the 48h clock, do an **incremental sync** after Hour 0–2 (findings), Hour 3–5 (prospects), Hour 5–8 (offer/outreach), and a **final sync** at Hour 42–48.

---

# FINAL SUCCESS CONDITION

The sprint is successful only when one of these happens:

### Primary

**Customer pays.**

### Secondary

Customer gives explicit written commitment to purchase at the agreed price, pending a normal administrative/procurement step.

Everything else is progress, not success.

---

# 14. URL OPPORTUNITY CAPTURE (ALTERNATIVE START)

This skill can also start from a **URL** instead of DOMAIN/LOCATION/PRICE.

When the user provides a **URL** (e.g., a company site, product page, industry report, regulator page, pricing page, or article), run **URL Opportunity Capture** once:

1. **Fetch + parse** the URL content (use `webfetch` / `exa` / `tavily` or browser if blocked). Extract:
   - **Domain** (industry + jargon in page)
   - **Target** (who the page sells to — company type/size, buyer persona, geography hints)
   - **Pricing opportunities** (current price, pricing model, gaps, willingness-to-pay signals, competitor pricing, penalty/cost of not buying)
   - **Expensive problems implied by the page** (jobs-to-be-done not met, complaints, limitations, regulatory requirements, operational bottlenecks visible on page)
   - **Evidence links** (quote page excerpts with URL citations)
2. **Infer sprint inputs** from the URL:
   - `DOMAIN` = inferred industry/domain from page
   - `LOCATION` = inferred geography (or ask if ambiguous — default to page's market)
   - `PRICE RANGE` = inferred from page pricing or adjacent comps (or set `TBD — propose 3 anchors`)
3. **Immediately start the normal 48h sprint** (§1-§13) using those inferred inputs — do not wait for separate confirmation unless inference confidence is low. State assumptions explicitly and allow user to correct.
4. **Output for this mode** (at top of report + chat):
   - Source URL + fetched title/date
   - Captured Domain / Target / Pricing Opportunities (bullet list with citations)
   - Inferred `48h Money In: [DOMAIN] | [LOCATION] | [PRICE]` with confidence note
   - Then proceed to §1 FIND THE MONEY as usual, logging URL evidence into Market Research Findings.

Example triggers:
- `48h Money In: https://example.com/pricing`
- `48h https://regulator.gov/new-rule-2026`
- `run 48h on this URL: https://...`

If the URL is blocked/paywalled, use fallback: text extraction via cache / `tavily` extract / browser, and note limitation.

---

# 15. SHIP TO GITHUB (FINAL BUILD STEP)

After the MVP is built and the customer has given a buying signal, the final step before demo is to **ship the solution to GitHub** so it is live, reproducible, and the customer can access it.

This step runs **after §5 BUILD**. It applies to the solution code repo (not the Obsidian vault — that syncs per §13).

## Step 1 — Seed + .env setup (run the setup script)

### Track A — Web SaaS
- The generator already created `scripts/seed-env.sh` (or `scripts/setup.ts`).
- Run it: `bash scripts/seed-env.sh` (or `npx tsx scripts/setup.ts`).
- It asks for: `NEXT_PUBLIC_CONVEX_URL`, `CONVEX_DEPLOYMENT`, `NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY`, `CLERK_SECRET_KEY`, `CLERK_WEBHOOK_SECRET`, `STRIPE_SECRET_KEY`, `NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY`, `STRIPE_WEBHOOK_SECRET`, `STRIPE_PRICE_CREDITS`, `NEXT_PUBLIC_SITE_URL`, `ADMIN_EMAIL`.
- It writes `.env.local` and `.env.production`, runs `npx convex codegen` + `npx convex dev --once --typecheck disable`, and reports readiness.
- On subsequent runs, it only validates existing `.env.local`.

### Track B — Mobile-only iOS
- The generator created `scripts/setup-ios.sh`.
- Run it: `bash scripts/setup-ios.sh`.
- It asks for: `REVENUECAT_IOS_API_KEY`, `FIREBASE_PROJECT_ID`, `APPLE_TEAM_ID`, `BUNDLE_ID`, product IDs (`PRO_MONTHLY`, `PRO_YEARLY`).
- It writes `.xcconfig`, validates `GoogleService-Info.plist` bundle match, runs `xcodebuild -resolvePackageDependencies`.

## Step 2 — Verify locally
- **Track A:** `npm run dev` → confirm `dev:majestic-wren-98` (or assigned name), register/login (Clerk) → buy credits (100 credits $1k) → use the workbench → vault/PDF/CSV. Run pre-flight checklist from §5.
- **Track B:** `xcodebuild run` (simulator) → sign in (Apple) → 3 free uses → paywall (RevenueCat sandbox) → core loop → history/share. Run pre-flight checklist from §5.

## Step 3 — Create GitHub repo (if needed) + push

```bash
# From the solution project root
git init 2>/dev/null

# Create repo on GitHub if it doesn't exist
gh repo create <REPO_NAME> \
  --public \
  --description "48h Money In: [DOMAIN] — [1-line value prop]" \
  --source=. \
  --remote=origin \
  --push
```

If the repo already exists, skip `--push` and push manually:

```bash
git remote add origin https://github.com/<OWNER>/<REPO_NAME>.git 2>/dev/null
git branch -M main
git add -A

# NEVER commit .env / keys — respect .gitignore
git restore --staged .env .env.local .env.production .xcconfig 2>/dev/null
git restore --staged "GoogleService-Info.plist" 2>/dev/null

git commit -m "48h money in: [DOMAIN] [LOCATION] [PRICE] — MVP shipped"
git push -u origin main
```

**Repo naming convention:**
```
48h-[domain-slug]-[location-slug]
# e.g. /48h-receipt-clearing-berlin
```

## Step 4 — Add README + deployment docs
- Generate `README.md` with: problem, buyer, solution, tech stack, setup instructions, seed script usage, and a link to the customer demo.
- Add `DEPLOY.md` if one-click deployment (Vercel / TestFlight) is not yet documented.
- Commit and push.

## Step 5 — Deploy to production (Track A) / TestFlight (Track B)
- **Track A:** Deploy Convex to prod (`npx convex deploy --yes`) + Vercel (`vercel --prod`), verify live URL works (Clerk login → Stripe checkout → webhook → Convex +100 → real workflow).
- **Track B:** Archive via `xcodebuild archive` + upload via Transporter; push to TestFlight internal tests immediately, then external for up to 10k testers.

## Rules
- **Never commit API keys, `.env.local`, `.env.production`, `.xcconfig`, or `GoogleService-Info.plist`.** Add them to `.gitignore` if the generator missed them.
- Verify `git status` is clean of secrets before each push.
- If `gh repo create` fails (repo exists), fall back to manual `git remote add` + push.
- Push at least once after seeds run and the app is E2E-verified — do not ship a broken repo.

---

# START COMMAND

When invoked with:

`48h Money In: [DOMAIN] | [LOCATION] | [PRICE RANGE] | [Web|iOS - optional, defaults to Web]`

**or**

`48h Money In: [URL]`  *(URL Opportunity Capture mode — see §14)*

**or**

`48h Money In mobile-only / iOS: ...` *(shorthand for Track B — SwiftUI + Firebase + RevenueCat)*

immediately run §0 INTAKE first.

Do not skip the four questions (domain, location, pricing, platform). Echo provided values, ask for missing ones, then start.

Start by finding **real problems being experienced today**, not by brainstorming products. When started from a URL, first run §14 capture, then §0 INTAKE gap-fill, then §1 FIND THE MONEY. After a buying signal is received and the MVP is built, always run §15 SHIP TO GITHUB to seed, set up .envs, create/push the repo, and deploy.
