# Offer: Backend Rescue Audit

## Who it's for

A technical founder, agency owner, or solo developer who has a Laravel/PHP project that is "on fire" — things are breaking, they don't know where to start, and they need someone to come in, assess the situation, and give them a clear action plan. This is the generalist version of the other audits.

## What pain it solves

- "Everything is breaking and I don't know where to start."
- "I inherited this project and I don't understand it."
- "We have multiple problems — code, infra, testing — and I need someone to prioritize."
- "I need a second pair of senior eyes to tell me what's actually wrong."

## Observable buying signals

- Developer or founder posting about frustration with their project (LinkedIn, X/Twitter, Reddit)
- Company hiring for a "rescue" or "cleanup" role
- Agency taking over a project from another agency (handover chaos)
- Solo developer posting about being overwhelmed or stuck
- Company about to launch but worried about stability

## What the client gets

1. A rapid assessment of the project's health across 4 areas:
   - Code quality (is it structured or chaotic?)
   - Testing (is there any safety net?)
   - Infrastructure (is the deployment stable?)
   - Critical issues (what's about to break?)
2. A prioritized "rescue plan" — what to fix first, what can wait, what to ignore
3. A 60-minute walkthrough call where you explain the findings
4. An optional follow-up: help implementing the top 1–2 fixes (separate engagement)

## What you actually do (delivery methodology)

### Day 1: Rapid scan
1. Get access to the codebase and any server/dashboard access available
2. Spend 2–3 hours doing a broad scan:
   - Directory structure (is it standard Laravel or heavily customized?)
   - Laravel version and PHP version
   - Number of routes, controllers, models (gives a sense of size)
   - Run `composer outdated` and `composer audit`
   - Check for tests: how many test files exist?
3. Note your first impressions: what looks good, what looks concerning

### Day 2: Deep dive on the scariest area
1. Based on Day 1, pick the area that looks most risky:
   - If no tests → focus on critical paths that are untested
   - If old Laravel version → focus on upgrade risks
   - If messy code → focus on the most complex/touched files
   - If infra concerns → focus on deployment and server setup
2. Spend the day understanding that area deeply
3. Document specific issues with file/line references

### Day 3: Quick checks on remaining areas
1. Do a 1–2 hour pass on each remaining area:
   - Code quality: are there god classes? Fat controllers? Service layer?
   - Testing: what's the coverage? What's critical and untested?
   - Infrastructure: what's the deployment process? Any monitoring?
   - Security: any obvious issues? (hardcoded credentials, debug mode, outdated packages)
2. Note the severity of each finding

### Day 4: Rescue plan
1. Write the prioritized rescue plan:
   - **Critical (fix this week):** security issues, things about to break, data loss risks
   - **High (fix this month):** missing tests on critical paths, deployment risks, performance issues
   - **Medium (fix this quarter):** code organization, technical debt, monitoring gaps
   - **Low (fix when you can):** nice-to-haves, code style, minor optimizations
2. For each item, include: what it is, why it matters, recommended fix, estimated effort

### Day 5: Walkthrough and handoff
1. Schedule the 60-minute walkthrough call
2. Walk the client through the rescue plan
3. Answer questions and help them prioritize based on their constraints
4. Offer to help implement the top 1–2 fixes as a follow-up engagement

## Required access and tools

- Read access to the codebase
- Optional: server/dashboard access (if infra is part of the assessment)
- Local PHP/Laravel environment
- Your 14+ years of backend development experience

## Skills you need

- Broad Laravel/PHP expertise (you have this)
- Ability to quickly assess code quality and identify critical issues
- Infrastructure knowledge (Docker, servers, CI/CD — you have this)
- Communication: explaining technical risk to non-technical people
- Prioritization: knowing what's urgent vs. what can wait

## Can I deliver this? Self-assessment checklist

- [ ] I can quickly scan a Laravel codebase and identify the biggest risks
- [ ] I can assess code quality, testing, infrastructure, and security in a broad pass
- [ ] I can write a clear, prioritized action plan
- [ ] I can explain technical risks to both technical and non-technical audiences
- [ ] I can identify which problems are urgent and which can wait
- [ ] I can do this in 5 working days or less

If you check 5+ boxes, you can deliver this offer.

## Delivery risk level: LOW

Read-only assessment. You're not changing anything — you're providing clarity and a plan.

## Suggested starter price range

€750–1,500 for the full audit + rescue plan + walkthrough.

- €750 for a small project (single app, focused scope)
- €1,500 for a larger or more complex project (multiple areas of concern)

This is intentionally priced lower than the specialized audits because it's a broader, less deep assessment. It's a great entry point — many clients will want to follow up with a specialized audit or implementation.

## What proof/content can come from it

- A YouTube video: "I rescued a Laravel project that was on fire — here's what I found"
- A LinkedIn post: "The 3 things I check first when I inherit a messy Laravel project"
- A case study: before/after project health metrics
- A reusable "project health checklist" as a lead magnet

## When NOT to sell this offer

- The project is not actually in trouble (if it's healthy, sell the specialized audits instead)
- The client expects you to fix everything as part of the audit (this is assessment only)
- The project uses a stack you don't know (e.g. it's not Laravel/PHP)
- You don't have 5 consecutive days available
