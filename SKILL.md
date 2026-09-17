---
<name: 48h
description: 48-hour sprint to land a first paying customer (aka 48h Money In). Always starts by asking domain(area), location/region, pricing target, and platform (Web SaaS vs mobile). Supports Web (Next.js+Convex+Stripe) and mobile ideas (Flutter+Firebase+RevenueCat IAP, iOS+Android). Autonomously builds and deploys the app (production deploy requires human approval) and operates it like real business ops — maintenance, optimization, marketing, sales, CRM — for new or existing 48h apps. Use when the user invokes "48h: [DOMAIN] | [LOCATION] | [PRICE RANGE]" or provides a URL to capture domain/target/pricing opportunities, or asks to find/validate/sell a solution to a real expensive problem and close a paying customer within 48 hours, or asks to build/deploy/operate/maintain/market/sell an existing 48h app. Do not use for long product development or general brainstorming.
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

> **Problem → Buyer → Validation → Solution → Demo → Offer → Payment → Autonomous Build → Approved Deploy → Operate**

The clock starts immediately.

The agent **autonomously builds, tests, and prepares deployment** for new or existing 48h apps. **Production deployment always requires explicit human approval** — never deploy to prod, push to TestFlight external, or run destructive migrations without a `deploy:approve` confirmation. Business operations after ship (maintenance, optimization, marketing, sales, CRM) run autonomously as §16 OPERATE.
---

# 0. INTAKE — ASK DOMAIN, LOCATION, PRICING FIRST (MANDATORY)

Do NOT start research until you have these three inputs confirmed.

If the user invoked with `48h: [DOMAIN] | [LOCATION] | [PRICE RANGE] | [Web|Mobile]` and domain/location/price are clear (platform defaults to Web if unstated), echo them back in one line and start the clock.

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
   - For mobile (Track B): answer as IAP subscription target, e.g. `$4.99–$9.99/mo or $39–$79/yr`.

4. **Platform?** — Web SaaS or mobile?
   - Options: `Web SaaS (Next.js + Convex + Stripe)` (default) / `Mobile (Flutter + Firebase + RevenueCat, iOS + Android)`
   - Ask this always — do not infer from domain alone. If user says `mobile`, `iOS`, `Android`, `iPhone`, `Flutter`, `App Store`, `Play`, route to Track B (§5 Track B).
   - If invocation already states platform (e.g. `mobile`, `iOS`, `Android`, `Flutter`), echo it and skip asking.

Rules:
- Ask all missing inputs in ONE batch, not one-by-one.
- Never silently infer location or pricing — a wrong guess wastes the 48h.
- Company type/size is optional bonus (infer from domain unless B2B enterprise — then confirm buyer).
- Platform routing: `Web` → §5 Track A, `Mobile` → §5 Track B. State the chosen track explicitly.
- Once answered, restate as: `48h: [DOMAIN] | [LOCATION] | [PRICE] | [Web|Mobile] — clock started` and proceed to §1.
- Start the ledger: record `START_UTC` (now) and `DEADLINE_UTC = START_UTC + 48h`, create `$OBSIDIAN_VAULT/48h/ledger-<YYYY-MM-DD>-<domain>.md` with inputs + deadline, and tell the user the exact deadline.
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

# 5. AUTONOMOUS BUILD + APPROVED DEPLOY (AFTER BUYING SIGNAL)

If the problem is validated, **autonomously build the smallest possible solution** — do not wait for step-by-step permission for code, tests, seeds, or local preview. Ask the human only for: missing API keys / secrets, and explicit production-deploy approval (§15).

Autonomy rules:
- **Build without asking:** scaffold, spec, code, seed scripts, `npm run build`, `npm run test:unit` + `npm run test:e2e` (Track A) / `flutter analyze` + `flutter test` (Track B), local `npm run dev` / `flutter run` on device, Cloudflare Tunnel preview, README/DEPLOY docs.
- **Stop and ask before:** `npx convex deploy --yes`, Docker image push + VPS deploy (`docker compose pull && docker compose up -d`), Play internal / TestFlight external upload, store submission, any prod DB migration / secret rotation / domain DNS change, any spend >$0 (paid services), any mailbox/social send (still manual per §4/§11).
- **Deploy approval gate (mandatory wording):** present `Deploy plan: [targets + migration + rollback] — reply deploy:approve to ship` and wait. Log approval (who/when/what) in chat + Obsidian report. Preview links (localhost, Tunnel `*.trycloudflare.com`, Firebase App Distribution, TestFlight internal, Docker preview) do NOT need approval; prod does.
- **Existing 48h apps:** if the user points at a repo/folder/live URL, treat it as the app — audit first (`build`/`test`/pre-flight checklist), then extend/fix in place. Never re-scaffold over it; infer DOMAIN/LOCATION/PRICE from code + URL capture (§14) and confirm in one line.

**Builder stack** (mandatory) — code only via these TUIs:
* opencode TUI
* kilo TUI
* cline TUI

Infra/services (allowed alongside): GitHub, Supabase, Docker ($5 VPS), Vercel, Cloudflare, APIs, LLMs, automation platforms, existing SaaS, open-source software. No other coding agent (Claude Code, Cursor, etc.) unless the human explicitly approves it.

Model approval gate (mandatory):
- Use **human-approved models only** inside the TUIs. Before starting build (and before any model switch, paid model, or preview/experimental model), present `Model plan: [TUI + model + task scope] — reply model:approve to proceed` and wait.
- Default to already-approved models; never auto-switch, auto-upgrade, or burn paid inference without `model:approve`.
- Log TUI + model per task in chat + Obsidian report (e.g. `opencode / [model] — scaffold`, `cline / [model] — fix checkout`).

Use AI aggressively within the approved TUI + model.

The objective is not to demonstrate engineering ability.

The objective is to create **customer value**.

Prefer:

> Working ugly prototype

over:

> Beautiful unfinished product.

Build only what is required to demonstrate the promised outcome.

### Track A — Web SaaS (default) — Spec-Driven via spec-kit + Hallmark UI

When you do build, **always kick off Track A with spec-driven development: install spec-kit + Hallmark first, then spec → Hallmark UI → code.** After building, run §15 SHIP TO GITHUB to seed, set up .envs, and push to a GitHub repo (created if needed).

- **0. Kickoff installs (mandatory, first commands in fresh project root):**
  ```bash
  # spec-kit — Spec-Driven Development (https://github.com/github/spec-kit)
  # Prerequisites: Python 3.11+ and uv
  uv tool install specify-cli
  # Scaffold spec-kit for your builder TUI (integration keys: opencode | cline | kilocode)
  specify init my-app --integration opencode
  # Hallmark — owns ALL UI (anti-AI-slop design skill, https://github.com/nutlope/hallmark)
  npx skills add nutlope/hallmark
  ```
  Verify: `specify integration status` reports ok + Hallmark present (`ls ~/.claude/skills/hallmark/ .cursor/rules/hallmark.mdc ~/.codex/skills/hallmark/ 2>/dev/null`) — re-run installers if missing. (`specify integration list` shows all agent keys; inside an existing checkout follow spec-kit's existing-project guide.) Never write app code before the spec exists and Hallmark is installed. Code only via opencode/kilo/cline TUIs (§5 builder stack) with `model:approve`.
- **Spec first (spec-kit SDD):** invoke the `/speckit-*` skills in the agent chat, one at a time — `/speckit-constitution` once per project (code-quality/testing principles), then per feature `/speckit-specify` (feed it the §3 SELECT ONE output: problem → buyer → scope → success criteria) → `/speckit-plan` → `/speckit-tasks` → `/speckit-implement` → `/speckit-converge`, repeating implement → converge until it reports **Converged**. These are agent-chat skills, not terminal commands. Spec is the source of truth; Hallmark builds UI from it. Optional extensions: `specify extension add assess` (idea intake → research → define → shape → decide, ending in go / clarify / kill — use at §2–§3 to kill weak ideas with evidence) and `specify extension add bug` (`/speckit-bug-assess → fix → test`, reports in `.specify/bugs/` — use in §16 Maintain).
- **Frontend — Hallmark owns ALL UI:** **Next.js 16 App Router + Tailwind + shadcn/ui + full landing page** — marketing landing (hero with **single primary CTA** `Upload 10 [ITEM]s — see [OUTCOME] →` only (e.g. `Upload 10 invoices — see cleared →` for a reconciliation domain), no secondary pricing hero button, problem → before/after, pricing 100 credits — $99 ($0.99/credit), social proof, FAQ) + app — fast to brand (logo/colors/subdomain, single `ShieldCheck` logo + App name, no extra icons), responsive, Docker-ready (`Dockerfile` + `docker-compose.yml`, deploys to a $5 VPS). **Hallmark ([live](https://www.usehallmark.com) · [github](https://github.com/nutlope/hallmark)) is responsible for building ALL UI — never hand-roll hero/landing styling.** Install above auto-detects: Claude Code `~/.claude/skills/hallmark/`, Codex `~/.codex/skills/hallmark/`, Cursor `.cursor/rules/hallmark.mdc`; then just ask for UI — hallmark attaches via `hallmark.observe()`. 48h workflow: `hallmark audit` current page (ranked punch list, **no edits**) → Hallmark picks the theme that best matches the solution → `hallmark build` with that theme (macrostructure → theme → enrichment; stamped, slop-tested; refuses repeating last 3 macrostructures) → apply tokens to landing + `/app`. Extra verbs: `hallmark study <URL|screenshot>` → DNA card (`lock the DNA` → portable `design.md`, never copies pixels); `hallmark redesign` keeps content/brand, changes bones. **Theme selection — Hallmark chooses one best-fit theme from the catalog/showcase and applies it (do not default blindly to Tally):**
  - `Hum` — Bubble guided sourdough app (editorial/playful consumer)
  - `Cobalt` — Distil content-extraction API (modern-minimal dev/API)
  - `Carnival` — Cold Snap record-label EP (bold music/culture)
  - `Lumen` — Cinder AI reasoning tool (atmospheric AI)
  - `Custom` — Ferns & Fathom tea menu / Press Quaternary type studio / Cascadia Nightjar / Mend Assembly (brief carries creative intent no catalog theme fits)
  - `Garden` — Hollowback Apiary honey farm (organic/editorial)
  - `Riso` — Off-Register risograph print fair (print/brutalist)
  - `Tally` — SaaS product page, modern-minimal (default ONLY for generic B2B SaaS fix-pack)
  - `Wayfare` — travel booking, atmospheric
  - `NAJM` — Moroccan fashion brand
  - `Hyperlane` — developer infrastructure
  - Full 21-theme catalog also available: Specimen, Atelier, Brutal, Newsprint, Studio, Manifesto, Terminal, Midnight, Almanac, Garden, Riso, Sport, Bloom, Coral, Cobalt, Aurora, Editorial, Carnival, Lumen, Hum, Grid (press T on the Hallmark demo site to preview) — pick best-fit, state `Macrostructure: <name>. Theme: <name>. Differs from last on: <axes>.` before code. Obey 8 foundations (display+body font pair, never Inter-everywhere; OKLCH 1 anchor hue, accent <5%; spacing multiples of 4; asymmetric biased layout; exponential ease-out + reduced-motion; distinct voice; display/body/label hierarchy) and avoid the 5 slop tells audit flags (purple-gradient hero → solid + single accent; Inter-as-display; centred-everything; icon-tile feature cards; generic AI nav). **Codebase must follow Clean Architecture** — `src/domain` (entities/use-cases, no framework), `src/application` (services, ports), `src/infrastructure` (Convex/Clerk/Stripe/PDF adapters), `src/presentation` (Next.js app routes + shadcn components) → dependency rule points inward, Hallmark tokens live only in presentation. **Use proper logo from icon library** — `lucide-react` `ShieldCheck` single + wordmark, token-colored. **Top menu (N5 pill → N1b for Hum) must show** `logo - App name - Buttons (App, Admin if admin) - Logged user + balance (if logged)` — Clerk `<UserButton>` / `useUser()` avatar + email + credits badge + **Buy Credits → Stripe Checkout** → redirect back to `/app` (success_url=`/app?credits=added`), keep `stripe listen` open; also show **Logout/Login**. **Admin link must NOT appear in public** — only visible to admin user. **Footer must be generic** — `About`, `Terms`, `Privacy`, `Contact`, `Sitemap`, `Robots` (all 200, not 404), no `White-label experiment — 1 customer · 1 day` text.
- **Auth:** **Clerk** — hosted auth (sign-in/up, orgs), webhook → Convex `users`, **admin user for me** (seeded via `ADMIN_EMAIL` env, role=admin). No custom auth.
- **Backend:** **Convex** — real tables (no dummy data), schema in `convex/schema.ts` (tenants, users, credits, vault, submissions + [DOMAIN] tables, e.g. invoices), file storage for XML/PDF, realtime queries. **Just put API keys in `.env.local` and it is ready — max 1 minute setup** (`NEXT_PUBLIC_CONVEX_URL`, `CLERK_*`, `STRIPE_*`). **Push live:** after seed, run `npx convex codegen` + `npx convex dev --once --typecheck disable` (dev at `dev:<your-deployment>`, prod via `npx convex deploy --yes`) — ensure DB, schema, indexes, and functions (`credits:getBalance/getOrCreate/consume/addCredits`) are built and deployed; verify with `npx convex run credits:getOrCreate '{"clerkId":"test123"}'`. No seed stubs.
- **SEO (when creating app):** **Always include SEO** — Next.js Metadata API (title/description/canonical/OG/Twitter), `sitemap.ts`, `robots.ts`, `llms.txt`, JSON-LD (Organization + Product + FAQ), OG image (1200x630), `next-sitemap` or `next-seo`, and keyword-ready blog stub (`/blog`). Hallmark theme must not break SEO (semantic headings, alt text, meta).
- **Billing:** **Stripe — 1 fixed package, credit-based usage** — **100 credits — $99 ($0.99/credit)**, credits decrement per use (1 credit per [ITEM], e.g. invoice), **free 3 on signup**, customer portal + webhook (`stripe listen --forward-to localhost:3000/api/webhooks/stripe` kept open) → Convex `credits`/`subscriptions`. **Buy Credits in top menu goes to Stripe Checkout (100 credits, $0.99/credit) and on success redirects back to `/app` — webhook must update Convex DB (`credits` +100) and UI must reflect new balance immediately (no manual refresh).** No product-tier sprawl — one package only. **Offer framing for the deal (not product tiers):** sell the engagement as a paid Pilot ($99) or Enterprise ($99 + $99/mo); both deliver the same 100-credit package.
- **Docs:** **PDF + CSV generation** — server-side PDF (report, vault export) + CSV exports (queue, vault) — tested with real domain field names (replace with your [DOMAIN] fields).
- **Ops:** **Admin panel** — `/admin` (Clerk protected, `role=admin` from Convex) — manage customers, view submissions, trigger re-runs, see Stripe + credits logs, toggle per-tenant branding. Admin is your `ADMIN_EMAIL`.
- **Data:** **`/data` page (Clerk-protected, add to `createRouteMatcher`)** — full CRUD over the Convex tables (tenants, users, credits, vault, submissions + [DOMAIN] tables, e.g. invoices) — tenant-scoped queries (users see own tenant rows; `role=admin` sees all), realtime Convex queries, server-side validation, delete requires confirm + writes an audit entry. No dummy rows; empty state shows "no records yet" + CTA into the `/app` workflow.
- **Connect:** **`/connect` page (Clerk-protected)** — asks for the Composio API key and lets the user connect the Composio toolkit(s) that fit the solution (pick per §3 solution scope, max 2 toolkits for 48h). Connected account defaults to the logged-in user — per-user connections stored under their Convex `users` row, owner-only read; never commit keys, never expose `COMPOSIO_API_KEY` to the client (all Composio calls run server-side via Convex actions or Next route handlers). Scope boundary: `/connect` integrations serve the customer's solution workflow only — sprint outreach stays manual per §4/§11 (no Composio sends for prospecting, ever).
- **Ready to use (non-negotiable):** **Working & tested E2E before handoff — prod-like, no dummy checks, real implementation from 0-day.** After generation, `put keys in .env.local → max 1m setup → npm run dev →` announce and users can **register/login (Clerk) → buy credits (100 credits — $99, $0.99/credit, free 3 on signup) → start using (1 credit per [ITEM]) → vault/PDF/CSV** with no extra dev — **customer invited on day 0 can use the app immediately, no simulation stub.** **`/app` must be Clerk-protected** (`src/proxy.ts` clerkMiddleware + `createRouteMatcher(['/app(.*)','/admin(.*)','/data(.*)','/connect(.*)'])` → `auth.protect()`) **and must do login check + credits check + UI works as designed** — unauthed redirects to `/sign-in`, no credits shows “buy 100”, with credits shows **real workbench (upload → validation → real [DOMAIN] workflow via API → vault)** fully interactive, Hallmark-themed, responsive at 320/375/414/768. **No simulation — `/app` is the real implementation of the solution for your [DOMAIN] (not stub), customer can invite and use from 0-day.** **Stripe sandbox buy must update DB and UI: `checkout.session.completed` → Convex `credits` +100 via webhook, and `/app?credits=added` must refetch and show new balance without manual refresh.** **If seed ran before and `.env.local` is already valid, `npm run dev` just validates (checks Convex/Clerk/Stripe connectivity, no re-prompt).** Require `npm run build` + `npm run test:unit` + `npm run test:e2e` (real Clerk sign-up, real Stripe test checkout → webhook → Convex +100 → UI badge updates, real PDF download, login/credits UI assertions, real [DOMAIN] processing call) passing — **no `if (!key) use dummy` branches, no `simulate*` stub in prod path (e.g. `simulateClearance`).** Then run §15 SHIP TO GITHUB to create/push the repo and ship to a $5 VPS via Docker.
- **Seed script (after generation):** **Create `scripts/seed-env.sh` (or `scripts/setup.ts`) that asks you for API keys** — `NEXT_PUBLIC_CONVEX_URL`, `CONVEX_DEPLOYMENT`, `NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY`, `CLERK_SECRET_KEY`, `CLERK_WEBHOOK_SECRET`, `STRIPE_SECRET_KEY`, `NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY`, `STRIPE_WEBHOOK_SECRET`, `STRIPE_PRICE_CREDITS`, `COMPOSIO_API_KEY` (optional — server-side key for `/connect`; per-user connections still collected at runtime), `NEXT_PUBLIC_SITE_URL`, `ADMIN_EMAIL` — **you paste them, it writes `.env.local` and `.env.production` (or VPS/compose env), runs `npx convex codegen` + `npx convex dev --once --typecheck disable` (or `npx convex deploy --yes` for prod) + `npm run build` check, verifies `npx convex run credits:getOrCreate` (free 3), then reports `✓ ready — register/login → buy credits (100 credits $99, $0.99/credit, free 3) → start using` confirmation. On subsequent `npm run dev`, it only validates existing `.env.local` instead of re-asking.**
- **Tests:** unit tests colocated with source (`*.test.ts(x)`, Vitest) — `src/domain` use-cases + credit/billing math first (framework-free, trivially testable), then route handlers; scripts `npm run test:unit` (Vitest) + `npm run test:e2e` (existing E2E). Both green before handoff; CI runs unit on every push.
- **CI/CD (GitHub Actions):** scaffold `.github/workflows/ci.yml` (on push/PR: `npm ci` → lint + typecheck → `test:unit` → `build`) and `.github/workflows/deploy.yml` (`workflow_dispatch` only, targeting a `production` Environment with required reviewers — the GitHub-native `deploy:approve` gate): build + push Docker image to GHCR, `npx convex deploy --yes`, SSH `docker compose pull && docker compose up -d` on the $5 VPS. All secrets via GitHub Secrets / Environment secrets, never committed.
- **Preview:** **Cloudflare Tunnel (free)** — creates a secure, encrypted tunnel from your local machine to Cloudflare’s edge. Install `cloudflared` (`brew install cloudflared` / `npm i -g cloudflared`), then `cloudflared tunnel --url http://localhost:3000` while `npm run dev` is running to share a public `https://*.trycloudflare.com` link instantly (no deploy) for customer demo before the VPS deploy.
- **Pre-flight checklist (before `npm run dev` — prevents the repeat failures seen in past sprints):**
  1. **Convex URL:** `NEXT_PUBLIC_CONVEX_URL` has **no trailing `/`** (`https://xxx.convex.cloud` not `.../`), `src/components/ConvexClientProvider.tsx` does `raw.replace(/\/+$/,'')`; otherwise `wss://...//api/...` → `1006`.
  2. **Convex push:** `CONVEX_DEPLOYMENT=dev:<your-deployment>` matches URL (e.g. `dev:adjective-noun-123` — yours will differ; never commit someone else's deployment name), then `npx convex codegen` + `npx convex dev --once --typecheck disable` (dev) or `npx convex deploy --yes` (prod) — verify `npx convex run credits:getOrCreate '{"clerkId":"test123"}'` returns `balance:3` (free 3); if `Could not find public function`, re-push.
  3. **Middleware location:** Next 16 + `src/` → file must be `src/proxy.ts` (not `middleware.ts` or root) — `clerkMiddleware` + `createRouteMatcher(['/app(.*)','/admin(.*)','/data(.*)','/connect(.*)'])` → `auth.protect()`; both files → error `Both middleware and proxy file are detected`.
  4. **Clerk UI:** never `SignedIn`/`SignedOut` (removed in Core 3) and no `UserButton afterSignOutUrl` — use `useUser()` + `isLoaded ? !user ? Login/Sign up : UserButton + credits + Buy`; `src/middleware` deprecation `createRouteMatcher` → keep but note.
  5. **Stripe price:** `STRIPE_PRICE_CREDITS` may be `price_...` or `100` — `src/app/api/checkout/route.ts` must branch `isPriceId ? {price} : {price_data:{currency:"usd", product:"100 credits @ $0.99/credit", unit_amount:9900}}` ($99 for 100 → $0.99/credit); `success_url` must be `new URL(req.url).origin + "/app?credits=added"` (not `NEXT_PUBLIC_SITE_URL` prod on localhost). Webhook `src/app/api/webhooks/stripe/route.ts` must skip verification if `STRIPE_WEBHOOK_SECRET` is `...` placeholder, otherwise `whsec_...` from `stripe listen --forward-to localhost:3000/api/webhooks/stripe` must be kept open, and `/app?credits=added` must refetch Convex `getBalance` via realtime (no manual refresh).
  6. **Hero/Footer:** Hero has **single CTA** (`Upload 10 [ITEM]s — see [OUTCOME] →` only, no secondary pricing button) and footer is **generic** (`About`, `Terms`, `Privacy`, `Contact`, `Sitemap`, `Robots` all 200) — no `White-label experiment — 1 customer · 1 day` text; create `src/app/about|terms|privacy|contact/page.tsx` + `sitemap.ts` includes them, otherwise 404.

> Prompt hint: `spec-kit kickoff (uv tool install specify-cli + specify init --integration opencode|cline|kilocode + npx skills add nutlope/hallmark first, then /speckit-constitution once + /speckit-specify → plan → tasks → implement → converge until Converged) + Next.js 16 App Router + Tailwind + shadcn/ui + Hallmark owns ALL UI (audit → best-fit theme from Hum/Cobalt/Carnival/Lumen/Garden/Riso/Tally/Wayfare/NAJM/Hyperlane/Custom → build; foundations: font-pair, OKLCH 1-hue, asymmetric, no slop) + full landing + Clean Architecture (domain/application/infrastructure/presentation) + Clerk (admin user, /app Clerk-protected with login + credits check, top menu logo - App name - Buttons - Logged user + balance) + Convex (real tables, no dummy, 1m setup, prod-like, push live via convex dev --once + deploy) + SEO (metadata/sitemap/robots/JSON-LD/OG/llms.txt) + Stripe (100 credits — $99, $0.99/credit, free 3 on signup, top-menu Buy Credits → Stripe → /app?credits=added, keep stripe listen) + PDF/CSV + /admin + /data (CRUD over Convex tables, tenant-scoped) + /connect (Composio API key, per-user default, solution-fit toolkits, server-side only) + proper logo (lucide ShieldCheck) + seed script (asks for CONVEX/CLERK/STRIPE/COMPOSIO keys → writes .env.local + prod → codegen + dev --once + build → reports ready, 100 credits $99) + unit tests (Vitest colocated, test:unit) + GitHub Actions (ci.yml on push/PR + deploy.yml on dispatch to production env = deploy:approve) — working & tested E2E prod-like, real implementation (100 credits $0.99/credit, /app real [DOMAIN] workflow from 0-day, no simulation), preview via Cloudflare Tunnel then Docker-ship to a $5 VPS.`

This keeps §5 Track A narrow (one fix-pack schema, one customer tenant) while leaving monetization + audit trails production-ready.

### Track B — Mobile (Flutter + Firebase + RevenueCat, iOS + Android)

Use when §0 Platform = `Mobile`, or the idea only makes sense as a phone app (camera, push, widgets, health sensors, offline-first, store distribution). One Flutter codebase ships to both iOS and Android. Do NOT force the Web SaaS stack onto a mobile idea.

When you do build, **suggest generating the app spec-first** (same SDD discipline as Track A: `/speckit-specify` with problem → buyer → scope → success criteria → paywall), then build with Flutter (single codebase, both stores):

- **Spec first:** `/speckit-specify` writes the 48h mobile fix-pack spec (problem → user → single core loop → paywall → success metric) before code — matches §3 SELECT ONE. Scope to ONE core loop + paywall, nothing else.
- **Frontend:** **Flutter (stable, Dart 3+)** — single codebase for iOS + Android, max 3 tabs (Core loop + History/Vault + Settings) via `BottomNavigationBar`, Material 3 with Cupertino-adaptive widgets where idiomatic, `Semantics` accessibility + reduced-motion support, light/dark ready. No per-platform native code unless a plugin forces it.
- **Architecture:** **Clean Architecture** — `lib/domain` (entities/use-cases, no framework), `lib/data` (Firebase repositories), `lib/presentation` (Flutter widgets + state, no business logic). Dependency rule points inward. No business logic in widgets.
- **Auth + Backend:** **Firebase** — Firebase Auth (Sign in with Apple on iOS + Google Sign-In on Android; anonymous → upgrade path allowed for 48h demo), Cloud Firestore (real collections: `users`, `workspaces`, `items/submissions`, `entitlements`, `events` — no dummy data), Firebase Storage (images/PDFs), Cloud Functions (TS, 2nd gen) for webhooks + server-side validation, FCM push, Crashlytics + Analytics from day 0. **Run `flutterfire configure` and it is ready — max 5 minute setup** (`lib/firebase_options.dart` generated for both platforms). Security Rules locked-down (owner-only read/write, `request.auth != null`), Firestore indexes committed (`firestore.indexes.json`), verified with emulator (`firebase emulators:start`) before prod push.
- **Billing (non-negotiable):** **Store In-App Purchase on both platforms, subscription managed with RevenueCat (Flutter SDK)** — NO Stripe, NO custom billing, NO web checkout bypass (store rules). Setup: 1 monthly + 1 annual product in **both** App Store Connect and Google Play Console (e.g. `pro_monthly $7.99/mo`, `pro_yearly $59.99/yr` — adjust to §0 pricing target), both mirrored to the RevenueCat `pro` entitlement, `Purchases.configure(apiKey)` + `logIn(appUserID)` on auth, paywall triggered after 3 free uses (mirror of Track A free-3 pattern), restore-purchase in Settings, sandbox tested with StoreKit Configuration file (iOS) + Play license testers (Android) + RevenueCat sandbox. Webhook: RevenueCat → Cloud Function → Firestore `entitlements` (never trust client-side `isPro` alone). Gating: no entitlement → paywall sheet, with entitlement → full core loop.
- **Seed script (after generation):** Create `scripts/setup-mobile.sh` that asks for `REVENUECAT_API_KEY` (one key, both stores), `FIREBASE_PROJECT_ID`, `ANDROID_APPLICATION_ID`, `IOS_BUNDLE_ID`, product IDs (`PRO_MONTHLY`, `PRO_YEARLY`), then runs `flutterfire configure` + `flutter pub get` + validates `lib/firebase_options.dart` covers both platforms + `firebase use --add` check, then reports `✓ ready — run → sign in → 3 free uses → paywall (RevenueCat sandbox) → core loop → history/share` confirmation. On subsequent runs it only validates, never re-asks.
- **Tests + CI/CD (GitHub Actions):** unit + widget tests in `test/` (`flutter test`), `flutter analyze` clean, no `isPro` bypass; scaffold `.github/workflows/ci.yml` (on push/PR: `flutter analyze` → `flutter test` → `flutter build appbundle --release`); distribution lane via `workflow_dispatch` to the Firebase App Distribution tester group (= the `deploy:approve` gate for mobile). Secrets via GitHub Secrets, never committed.
- **Preview + distribution (48h-safe):** NO store review on the critical path — demo via `flutter run` on a real device + Screen Recording, then **Firebase App Distribution (iOS + Android testers, available in minutes) → Play internal track / TestFlight external (up to 10k)**. Customer invited on day 0 can use the app immediately via App Distribution, no review stub. Release with `flutter build apk --release` / `flutter build appbundle` / `flutter build ipa`; version bump per upload.
- **Ready to use (non-negotiable):** **Working & tested E2E before handoff — prod-like, no dummy checks, real implementation from 0-day.** After generation, `bash scripts/setup-mobile.sh → flutter run on a real device →` announce and users can **sign in → 3 free uses → paywall (RevenueCat) → subscribe (sandbox) → core loop → history/share/export** with no extra dev. **No `isPro = true` debug bypass in release path, no `simulatePurchase` stub in prod path.** Then run §15 SHIP TO GITHUB to create/push the repo and distribute via Firebase App Distribution. Require `flutter analyze` + `flutter test` (real Auth sign-in, real RevenueCat sandbox purchase → Firestore `entitlements/pro=true` → paywall unlocks, real export/share) passing.
- **Pre-flight checklist (before `flutter run`):**
  1. **IDs match:** `ANDROID_APPLICATION_ID` == Play Console == Firebase Android app == RevenueCat app config, AND `IOS_BUNDLE_ID` == App Store Connect == Firebase iOS app == RevenueCat app config; otherwise Auth/push/IAP all fail silently.
  2. **Auth providers:** Sign in with Apple (capability ON + App ID configured) + Google Sign-In (SHA-1/SHA-256 registered in Firebase); matching providers enabled in Firebase Auth.
  3. **RevenueCat products:** `pro_monthly`/`pro_yearly` exist in **both** App Store Connect and Play Console (draft/Ready to Submit minimum) AND linked to the `pro` entitlement in RevenueCat; StoreKit config file + Play license testers cover both for local testing.
  4. **Firestore rules:** `firebase deploy --only firestore:rules` pushed; emulator test passes for owner-only + entitlement-gated reads.
  5. **Paywall copy:** price + trial/terms + `Restore Purchases` + Privacy/Terms links (both stores reject without them); no `Subscribe` button that does nothing.

> Prompt hint: `mobile fix-pack: Flutter (stable, iOS + Android, 3-tab max) + Clean Architecture (domain/data/presentation) + Firebase (Auth Apple + Google, Firestore real collections, Storage, Functions 2nd gen, FCM, Crashlytics, flutterfire configure) + RevenueCat (pro entitlement both stores, pro_monthly + pro_yearly, 3 free uses → paywall, sandbox both platforms, webhook → Firestore entitlements) + scripts/setup-mobile.sh (asks REVENUECAT/FIREBASE/IDs keys → flutterfire configure → pub get → reports ready) + flutter test + flutter analyze + GitHub Actions (ci.yml on push/PR + App Distribution lane on dispatch = deploy:approve) — working & tested E2E prod-like, real core loop from 0-day, no simulation, distribute via Firebase App Distribution → Play internal / TestFlight external (no store review on critical path).`

Track selection rule: §0 Platform decides. Web → Track A only. Mobile (Flutter, iOS + Android) → Track B only. Never mix Stripe into mobile or RevenueCat into Web. Landing page for Track B = store listing assets (subtitle, screenshots plan, paywall copy for both stores) + optional one-page web teaser, not a full Next.js site.

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

### Clock tracking + ledger (mandatory)

- The ledger lives at `$OBSIDIAN_VAULT/48h/ledger-<YYYY-MM-DD>-<domain>.md`, created at intake (§0) with inputs, `START_UTC`, and `DEADLINE_UTC`.
- Append one entry at **every phase boundary**: phase, started/ended UTC, elapsed, remaining, key outcome.
- Every status report to the user **leads with**: `Clock: HH:MM remaining — deadline <DEADLINE_UTC> (ledger: <link>)`.
- Warn the user explicitly at **24h left, 8h left, and 2h left** — state what must be true by the deadline.
- If the deadline passes with no payment or written commitment: **stop building**, write the final outcome report, close the sprint. Never drift past 48h silently.

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

`HH:MM remaining — deadline <DEADLINE_UTC> (ledger: <link>)`

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

Save the report as a dated note in the Obsidian vault (e.g., `48h-2026-09-01.md`) and also under `48h/` if the sprint is domain-specific (e.g., `48h/48h-YYYY-MM-DD-domain.md`). Link it from the relevant project or daily note. Use the `obsidian-wiki-ingest` or `wiki-capture` skill if available.

### Vault git sync — required after report generation

The Obsidian vault (`$OBSIDIAN_VAULT`) is a git repo synced to its `origin/main`. **Whenever the vault gains or edits markdown files, you MUST commit and push.**

One-time setup per machine (use your own vault path and identity):

```bash
export OBSIDIAN_VAULT="/path/to/your/vault"  # persist in ~/.zshrc
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

After writing the report (and at each major stage if files were created), run:

```bash
: "${OBSIDIAN_VAULT:?OBSIDIAN_VAULT is not set — see one-time setup above}"
cd "$OBSIDIAN_VAULT"

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
   - Inferred `48h: [DOMAIN] | [LOCATION] | [PRICE]` with confidence note
   - Then proceed to §1 FIND THE MONEY as usual, logging URL evidence into Market Research Findings.

Example triggers:
- `48h: https://example.com/pricing`
- `48h: https://regulator.gov/new-rule-2026`
- `run 48h on this URL: https://...`

If the URL is blocked/paywalled, use fallback: text extraction via cache / `tavily` extract / browser, and note limitation.

---

# 15. SHIP TO GITHUB + APPROVED DEPLOY (FINAL BUILD STEP)

After the MVP is built and the customer has given a buying signal, the final step before demo is to **autonomously ship the solution to GitHub** so it is live, reproducible, and the customer can access it. **Git push + preview is autonomous; production deploy waits for human approval.**

This step runs **after §5 BUILD**. It applies to the solution code repo (not the Obsidian vault — that syncs per §13). It applies to **new scaffolds and existing 48h apps** (repo path, live URL, or TestFlight app — audit in place, then ship).

## Step 1 — Seed + .env setup (run the setup script)

### Track A — Web SaaS
- The generator already created `scripts/seed-env.sh` (or `scripts/setup.ts`).
- Run it: `bash scripts/seed-env.sh` (or `npx tsx scripts/setup.ts`).
- It asks for: `NEXT_PUBLIC_CONVEX_URL`, `CONVEX_DEPLOYMENT`, `NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY`, `CLERK_SECRET_KEY`, `CLERK_WEBHOOK_SECRET`, `STRIPE_SECRET_KEY`, `NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY`, `STRIPE_WEBHOOK_SECRET`, `STRIPE_PRICE_CREDITS`, `COMPOSIO_API_KEY` (optional — server-side key for `/connect`), `NEXT_PUBLIC_SITE_URL`, `ADMIN_EMAIL`.
- It writes `.env.local` and `.env.production`, runs `npx convex codegen` + `npx convex dev --once --typecheck disable`, and reports readiness.
- On subsequent runs, it only validates existing `.env.local`.

### Track B — Mobile (Flutter, iOS + Android)
- The generator created `scripts/setup-mobile.sh`.
- Run it: `bash scripts/setup-mobile.sh`.
- It asks for: `REVENUECAT_API_KEY`, `FIREBASE_PROJECT_ID`, `ANDROID_APPLICATION_ID`, `IOS_BUNDLE_ID`, product IDs (`PRO_MONTHLY`, `PRO_YEARLY`).
- It runs `flutterfire configure` + `flutter pub get`, validates `lib/firebase_options.dart` covers both platforms.

## Step 2 — Verify locally
- **Track A:** `npm run dev` → confirm `dev:<your-deployment>`, register/login (Clerk) → buy credits (100 credits $99) → use the workbench → vault/PDF/CSV. Run pre-flight checklist from §5.
- **Track B:** `flutter run` (real device) → sign in → 3 free uses → paywall (RevenueCat sandbox) → core loop → history/share. Run pre-flight checklist from §5.

## Step 3 — Create GitHub repo (if needed) + push

```bash
# From the solution project root
git init 2>/dev/null

# Create repo on GitHub if it doesn't exist
gh repo create <REPO_NAME> \
  --public \
  --description "48h: [DOMAIN] — [1-line value prop]" \
  --source=. \
  --remote=origin \
  --push
```

If the repo already exists, skip `--push` and push manually:

```bash
git remote add origin https://github.com/<OWNER>/<REPO_NAME>.git 2>/dev/null
git branch -M main
git add -A

# NEVER commit secrets — respect .gitignore
git restore --staged .env .env.local .env.production 2>/dev/null
git restore --staged "google-services.json" "GoogleService-Info.plist" 2>/dev/null
git restore --staged android/key.properties "*.jks" "*-service-account.json" 2>/dev/null

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
- Add `DEPLOY.md` documenting the $5 VPS Docker deploy (no platform lock-in).
- Commit and push.

<## Step 5 — Deploy to a $5 VPS via Docker (both tracks) — REQUIRES deploy:approve
- **Track A:** Next.js `output: 'standalone'` multi-stage `Dockerfile` + `docker-compose.yml` (app + Caddy reverse proxy with auto-TLS). Push the image to GHCR (`ghcr.io/<owner>/<repo>:<sha>`), provision a $5 VPS (Docker + firewall 22/80/443), then deploy over SSH (`docker compose pull && docker compose up -d`). Deploy Convex to prod (`npx convex deploy --yes`), verify the live URL end-to-end (Clerk login → Stripe checkout → webhook → Convex +100 → real workflow), and confirm rollback works (previous image tag still available).
- **Track B:** `flutter build apk --release` / `flutter build appbundle` / `flutter build ipa` → Firebase App Distribution (day-0 testers) → Play internal track / TestFlight external. Any custom server components ship with the same Docker pattern above.
- **Approval gate:** autonomous work stops before this step. Present deploy plan + rollback, wait for explicit `deploy:approve`. After approval, deploy, verify, log result + approver in chat + Obsidian report. Never deploy on implied approval ("looks good", "ship it-ish" still needs explicit `deploy:approve`).

## Rules
- **Never commit API keys, `.env.local`, `.env.production`, `google-services.json`, `GoogleService-Info.plist`, `android/key.properties`, or service-account keys.** Add them to `.gitignore` if the generator missed them.
- Verify `git status` is clean of secrets before each push.
- If `gh repo create` fails (repo exists), fall back to manual `git remote add` + push.
- Push at least once after seeds run and the app is E2E-verified — do not ship a broken repo.

---

# 16. OPERATE — MAINTENANCE, OPTIMIZATION, MARKETING, SALES, CRM (NEW OR EXISTING APPS)

After ship (or on any existing 48h app the user points at), act as real business operations. Trigger with `48h operate: [REPO PATH | GITHUB URL | LIVE URL] [focus: maintain|optimize|market|sell|crm|all]`. Audit first, then run the requested lanes autonomously. All code lanes use the §5 builder stack (opencode/kilo/cline TUIs with `model:approve`). Production changes still need `deploy:approve`; content/outreach drafts never auto-send (§4/§11).

## 16.1 Maintain
- Triage: repro → failing test or log evidence → smallest fix → `build` + `test:unit` + `test:e2e` (Track A) / `flutter analyze` + `flutter test` (Track B) green.
- Uptime/hygiene: dependency bumps (one at a time), env/secret validation via seed scripts, Convex/Firestore rules + indexes verified, backups/exports smoke-tested (PDF/CSV, Storage).
- Log every fix in Obsidian report + CHANGELOG; open follow-ups as todos, not silent skips.

## 16.2 Optimize
- Conversion: hero single-CTA check, pricing clarity (100 credits — $99), signup → pay → first-value funnel, empty-states, 320/375/414/768 pass.
- Performance: `npm run build` size audit, image/OG budgets, Convex query indexes, Firestore read fan-out, cache where free (no paid infra without approval).
- Measure before/after (time, DSO, ticket %, churn signal) and report as Before → After like §7.

## 16.3 Market
- Ship landing/blog/SEO deltas (metadata, sitemap, robots, llms.txt, JSON-LD, OG image), Hallmark audit → theme build per §5 Track A.
- Draft launch assets as files + pastes: posts, screenshots plan, paywall/App Store copy (Track B), FAQ/objection handling. Never auto-post.

## 16.4 Sell
- Re-run §3–§4 on the live app: buyer, offer, 3-message manual outreach batches, demo script against prod preview.
- Proposal/pricing/payment-instruction pack per §10 Hour 42–48. No Composio/mailbox/social automation — ready-to-paste only.

## 16.5 CRM
- Track every prospect/customer in the app's own store (Convex `customers/interactions` or Firestore `customers/events` — no dummy rows) + mirror to Obsidian report (status: contacted/responded/demo/closed/lost).
- Owner-only access (`role=admin` / Firestore owner rules); never expose PII in logs, screenshots, or commits.

Operate loop output (§12 format): Current Objective / Evidence / Best Opportunity / Buyer / Offer / Next Action / Clock (use `Ongoing` outside the 48h window). Sync vault per §13 after each lane.

---

# START COMMAND

When invoked with:

`48h: [DOMAIN] | [LOCATION] | [PRICE RANGE] | [Web|Mobile - optional, defaults to Web]`

**or**

`48h: [URL]`  *(URL Opportunity Capture mode — see §14)*

**or**

`48h mobile: ...` *(shorthand for Track B — Flutter + Firebase + RevenueCat, iOS + Android)*

**or**

`48h operate: [REPO PATH | GITHUB URL | LIVE URL] [maintain|optimize|market|sell|crm|all]` *(Operate mode — see §16; works on new or existing 48h apps)*

**or**

`48h build|deploy|fix|market|sell [EXISTING APP]` *(lane shorthand — routes to §5/§15/§16 on the existing app in place)*

immediately run §0 INTAKE first (new sprint) — except Operate mode, which skips intake and starts with an app audit (stack, env, tests, buyer/offer) then runs the requested §16 lanes.

Do not skip the four questions (domain, location, pricing, platform) for new sprints. Echo provided values, ask for missing ones, then start.

Start by finding **real problems being experienced today**, not by brainstorming products. When started from a URL, first run §14 capture, then §0 INTAKE gap-fill, then §1 FIND THE MONEY. After a buying signal is received and the MVP is built, autonomously build + test + push to GitHub per §15, then **stop for `deploy:approve` before any production deploy**. After ship, continue with §16 OPERATE (maintenance, optimization, marketing, sales, CRM) on request or on `48h operate`.
