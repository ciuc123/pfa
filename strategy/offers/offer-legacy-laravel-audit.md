# Offer: Legacy Laravel Codebase Audit

## Who it's for

A technical founder, CTO, or engineering manager at a company (1–50 people) that has a Laravel/PHP codebase that has been built over time and is becoming hard to maintain, onboard onto, or ship features from.

## What pain it solves

- "Our codebase is a mess and nobody fully understands it anymore."
- "Every new feature takes longer than it should because we're afraid of breaking things."
- "We want to hire a new developer but onboarding them onto this code is going to be painful."
- "We know we have technical debt but we don't know where to start fixing it."

## Observable buying signals

- Hiring a senior Laravel developer (signal: onboarding pain, need someone who can handle legacy)
- Engineering blog post mentioning "refactoring" or "technical debt"
- Job post mentioning "legacy codebase" or "modernization"
- Company just raised funding and is about to scale engineering
- GitHub repo showing old Laravel version (e.g. Laravel 8 or 9 in 2026)
- Developer at the company posting about frustration with their codebase

## What the client gets

1. A written audit report (5–10 pages) covering:
   - Codebase structure assessment (controllers, services, models — is it organized or spaghetti?)
   - Dependency health (outdated packages, security vulnerabilities)
   - Test coverage assessment (what's tested, what's not, what's critical)
   - Database schema review (migrations hygiene, indexes, potential issues)
   - Top 5–10 prioritized issues with severity, effort estimate, and recommended fix
2. A 60-minute walkthrough call where you explain the findings and answer questions
3. A one-page "fix roadmap" showing what to tackle first, second, third

## What you actually do (delivery methodology)

This is the step-by-step of how you deliver this audit. You don't need to know everything in advance — this is the process.

### Day 1: Access and setup
1. Get read access to the codebase (GitHub/GitLab invite or a zip export)
2. Get a list of any specific concerns from the client (a 15-min call or email)
3. Clone the repo locally
4. Run `composer outdated` to check for outdated dependencies
5. Run `composer audit` to check for known security vulnerabilities
6. Check the Laravel version and compare to current stable

### Day 2: Codebase structure review
1. Read the directory structure — is it a standard Laravel app or heavily customized?
2. Look at the routes file (`routes/web.php`, `routes/api.php`) — how many routes, how complex?
3. Sample 3–5 controllers — are they fat controllers (business logic in controllers) or thin (logic in services)?
4. Check for service classes, action classes, or other organization patterns
5. Look at the models — are they anemic (just DB mapping) or do they have business logic?
6. Note any "god classes" (files over 300–500 lines)

### Day 3: Testing and database review
1. Run the existing test suite: `php artisan test` or `vendor/bin/phpunit`
2. Check test coverage: how many test files exist vs. how many controllers/models?
3. Look at the migrations folder — are there messy or repeated migrations?
4. Check for foreign key constraints, indexes, and potential N+1 query problems
5. Look at any seeders or factories

### Day 4: Configuration and deployment review
1. Check `.env.example` for configuration hygiene
2. Look at `config/` files for any custom or overridden settings
3. Check for environment-specific issues (hardcoded credentials, debug mode in prod config)
4. Look at the deployment setup (CI/CD config, Dockerfile, deployment scripts)

### Day 5: Report writing and walkthrough
1. Write the audit report using a template (we'll provide one)
2. Prioritize the top 5–10 issues by severity (critical, high, medium, low)
3. For each issue, write: what it is, why it matters, recommended fix, estimated effort
4. Create the one-page fix roadmap
5. Schedule the 60-minute walkthrough call
6. Deliver the report as a PDF or markdown document

## Required access and tools

- Read access to the codebase (GitHub/GitLab or zip)
- Local PHP/Laravel environment (you already have this)
- A markdown editor or Google Doc for the report
- Optional: PHPStan or Larastan for static analysis (run `composer require --dev nunomaduro/larastan` and `./vendor/bin/phpstan analyse`)

## Skills you need

- Reading and understanding Laravel/PHP code (you have 14+ years — yes)
- Identifying common code smells and anti-patterns (fat controllers, god classes, N+1 queries)
- Writing clear, actionable recommendations
- Basic static analysis tool usage (PHPStan — easy to learn in 30 minutes)

## Can I deliver this? Self-assessment checklist

- [ ] I can read a Laravel codebase and identify fat controllers, god classes, and missing service layers
- [ ] I can run `composer outdated`, `composer audit`, and `php artisan test`
- [ ] I can install and run PHPStan/Larastan
- [ ] I can write a clear, prioritized report with specific recommendations
- [ ] I can explain technical findings to a non-technical founder or a technical CTO
- [ ] I can do this in 5 working days or less

If you check 5+ boxes, you can deliver this offer. If you check fewer than 5, note which skills you need to learn before selling it.

## Delivery risk level: LOW

This is a read-only audit. You are not changing their code. The worst case is a report they don't act on — which is still valuable to them and low-risk for you.

## Suggested starter price range

€500–1,500 for the full audit + report + walkthrough call.

- €500 for a small codebase (1–2 years old, < 50k lines)
- €1,000 for a medium codebase (2–5 years old, 50k–150k lines)
- €1,500 for a large codebase (5+ years old, 150k+ lines, multiple modules)

## What proof/content can come from it

- A YouTube video: "I audited a real Laravel codebase — here's what I found" (anonymize the client)
- A LinkedIn post: "5 things I find in every legacy Laravel codebase"
- A case study: before/after metrics if the client acts on your recommendations
- The audit report itself can become a lead magnet (generalized version)

## When NOT to sell this offer

- The codebase is brand new (less than 6 months old) — there's nothing to audit yet
- The company has a strong senior team that already does regular code reviews
- The client expects you to fix everything (this is an audit, not implementation — upsell implementation separately)
- You don't have 5 consecutive days available in your schedule
