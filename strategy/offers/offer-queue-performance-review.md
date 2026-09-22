# Offer: Queue & Performance Review

## Who it's for

A technical founder, CTO, or engineering manager at a Laravel SaaS or app (1–50 people) that is experiencing performance issues — slow page loads, queue job failures, timeout errors, or scaling problems as traffic grows.

## What pain it solves

- "Our queue jobs keep failing or timing out."
- "The app gets slow under load and we don't know why."
- "We're hitting database performance issues as we scale."
- "Our background jobs are backing up and affecting users."
- "We need to scale but we're not sure our current architecture can handle it."

## Observable buying signals

- Job post mentioning "performance", "scale", or "high traffic" alongside Laravel
- Status page incidents or user complaints about slow responses
- Developer at the company posting about queue or performance issues
- Company just raised funding and expects traffic growth
- Engineering blog post about a post-mortem or performance incident
- App is on a platform like Forge/Vapor and they're hitting plan limits

## What the client gets

1. A performance assessment report covering:
   - Queue configuration review (driver, retries, timeouts, supervisor config)
   - Database query analysis (N+1 queries, missing indexes, slow queries)
   - Application-level performance issues (heavy controllers, synchronous processing, missing caching)
   - Infrastructure review (server size, PHP-FPM config, opcache)
2. A list of the top 5 performance bottlenecks, ranked by impact
3. Specific code-level recommendations for each bottleneck (with file/line references)
4. A 60-minute walkthrough call with the team
5. An optional follow-up: implementation of the top 2 fixes (separate engagement)

## What you actually do (delivery methodology)

### Day 1: Access and environment review
1. Get access to: codebase (read), server/Forge/Vapor dashboard (read), Laravel Telescope or logging (if available)
2. Check the queue configuration in `config/queue.php` and `.env`:
   - What queue driver are they using? (sync, database, Redis, SQS)
   - Are they using Redis? If not, that's likely the first recommendation
3. Check `config/` for cache, session, and database configuration
4. Check the server setup: PHP version, PHP-FPM workers, opcache status
5. Note the hosting setup (Forge, Vapor, custom server, Kubernetes)

### Day 2: Queue and job analysis
1. Look at all queue jobs in `app/Jobs/` — how many, how complex?
2. For each job:
   - Does it have a timeout set?
   - Does it handle failures and retries properly?
   - Does it do heavy database operations inside the job?
   - Are there any jobs that should be batched but aren't?
3. Check for queue supervisors and worker configuration
4. Look at the `failed_jobs` table if it exists — what's failing?
5. Check for any long-running console commands or scheduled tasks

### Day 3: Database query analysis
1. Enable Laravel Telescope (if not already installed) or check existing query logs
2. Look for N+1 query problems in controllers and services (search for lazy loading in loops)
3. Check the database schema for missing indexes on frequently queried columns
4. Look at the largest/most complex migrations
5. Run `EXPLAIN` on the most common queries if you have database access
6. Check for eager loading: `with()` vs lazy `->relationship` calls in loops

### Day 4: Application-level review
1. Check for synchronous operations that should be async (email sending, file processing, API calls in request lifecycle)
2. Look at middleware — is there anything heavy running on every request?
3. Check caching strategy: are they using cache for expensive queries or computations?
4. Look at the frontend: are they loading too much data per request? (large API responses, no pagination)
5. Check for any memory leaks or unbounded queries (fetching all records)

### Day 5: Report and walkthrough
1. Write the performance assessment report
2. Rank the top 5 bottlenecks by impact (high/medium/low) and effort to fix
3. For each bottleneck, write: what it is, why it's slow/broken, specific fix recommendation, file/line reference, estimated effort
4. Create a one-page "performance fix roadmap" (what to fix first, second, third)
5. Schedule the 60-minute walkthrough call

## Required access and tools

- Read access to the codebase
- Access to server/Forge/Vapor dashboard (read-only)
- Optional: database access for query analysis (read-only)
- Optional: Laravel Telescope or query logging
- Local PHP/Laravel environment
- MySQL Workbench or TablePlus (for database analysis if needed)

## Skills you need

- Understanding Laravel queue system, jobs, and workers (you have this)
- Database query optimization and N+1 detection (you have this)
- PHP-FPM and server configuration basics (you have this — Docker/K8s experience)
- Reading and profiling Laravel application code
- Using Laravel Telescope or Laravel Debugbar

## Can I deliver this? Self-assessment checklist

- [ ] I can identify N+1 queries in Laravel code
- [ ] I can review Laravel queue configuration and job structure
- [ ] I can analyze database queries and identify missing indexes
- [ ] I can read and understand PHP-FPM and server config
- [ ] I can install and use Laravel Telescope or Laravel Debugbar
- [ ] I can write clear, specific performance recommendations with code references
- [ ] I can do this in 5 working days or less

If you check 5+ boxes, you can deliver this offer.

## Delivery risk level: LOW

This is primarily a read-only review. You are not changing their code or infrastructure — you're identifying problems and recommending fixes. If they want you to implement fixes, that's a separate engagement.

## Suggested starter price range

€750–1,500 for the full review + report + walkthrough.

- €750 for a small app (simple queue setup, single server)
- €1,000 for a medium app (multiple job types, Redis, moderate complexity)
- €1,500 for a complex app (multi-server, Kubernetes, heavy queue usage, database analysis needed)

## What proof/content can come from it

- A YouTube video: "I found 3 N+1 queries killing a Laravel app's performance"
- A LinkedIn post: "The 5 most common Laravel performance mistakes I see in production"
- A case study: before/after response times or queue throughput
- A reusable "Laravel performance checklist" as a lead magnet

## When NOT to sell this offer

- The app is brand new with very little traffic (no performance issues yet)
- The performance problem is clearly frontend-related (JavaScript, images, CDN — not your expertise)
- The client has no server access and can't provide dashboard access
- The app uses a completely different stack (e.g. they're on serverless PHP and you don't know the platform)
