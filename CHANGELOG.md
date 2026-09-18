# Changelog — 48h skill

Follows the skill's own §16 guidance: log every change, no silent skips.

## Unreleased

- **Build discipline migrated from spec-kit to addyosmani/agent-skills (spec-kit retired):** kickoff is now `npx skills add addyosmani/agent-skills --all -y` (25 skills, 70+ agents — no `specify-cli`, no `.specify/`, no `/speckit-*`); lifecycle is `spec-driven-development` → `planning-and-task-breakdown` → `incremental-implementation` + `test-driven-development` → `debugging-and-error-recovery` → `code-review-and-quality` → `shipping-and-launch` (routed via `using-agent-skills`); idea kill discipline is `idea-refine` + `interview-me` (go/clarify/kill with evidence, replaces `assess` extension); bug lane is `debugging-and-error-recovery` Prove-It pattern (replaces `bug` extension + `.specify/bugs/` reports)
- Fixed broken SKILL.md frontmatter (`<name:` → `name:` — was failing YAML parse in `skills list`)

- Track A + Track B generate unit tests and GitHub Actions CI/CD: Track A gets colocated Vitest unit tests (`test:unit`) + `ci.yml` (push/PR) + `deploy.yml` (`workflow_dispatch` to `production` env = `deploy:approve` gate); Track B gets `flutter test` + `flutter analyze` + `ci.yml` + App Distribution lane on dispatch

- spec-kit pinned to official flow (github/spec-kit): `uv tool install specify-cli` + `specify init --integration opencode|cline|kilocode`, `/speckit-constitution` once + `/speckit-specify → plan → tasks → implement → converge` until Converged; extensions mapped (`assess` → §2–§3 kill/clarify/go, `bug` → §16 Maintain)

- Track A: mandatory spec-kit + Hallmark kickoff installs before any app code
- Track A: Hallmark owns ALL UI with best-fit theme selection (no blind Tally default)
- Track A: `/data` CRUD page (tenant-scoped) + `/connect` Composio page (per-user default, server-side only)
- Parameterized domain examples (`[ITEM]`/`[OUTCOME]`, invoices as labeled `e.g.`)
- Protected routes extended: `/app`, `/admin`, `/data`, `/connect`
- Autonomy rules updated to Docker VPS / Flutter terminology; duplicate infra line merged

## 2026-09-17

- Stripe $99 package (100 credits, $0.99/credit, free 3); Flutter Track B (iOS + Android); 48h naming; clock ledger; $5 VPS Docker deploy
- Skill audit fixes: portable vault setup, Next.js 16, pricing consistency
- Repo renamed `48h-money-in` → `48h` (old links redirect); README badges, links, install paths updated

## 2026-09-15

- README with comprehensive skill documentation (tracks, clock, decision rules, ship steps)

## 2026-09-14

- §15 SHIP TO GITHUB — seed, .env setup, repo push

## 2026-09-08

- Full SKILL.md + README with GitHub badges + MIT LICENSE (flat shields style)
