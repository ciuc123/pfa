# Buying Signals — observable triggers that a team needs technical help

These are the observable, publicly visible events that indicate a company or team has a pain you can solve. A buying signal is not "they use Laravel" (that's a filter). A buying signal is something that has *changed* or is *happening right now* — a trigger event that creates urgency.

How to use this file:
- When researching prospects, look for one of these signals per prospect.
- Copy the exact wording of the signal into your tracking sheet.
- The signal becomes the first line of your outreach message ("Noticed you...").

---

## Signal type 1: Hiring

The strongest signal. A company spending money to hire is actively investing in an area where they have a gap.

| Signal | What it tells you | Where to find it | Search example |
|---|---|---|---|
| Hiring a senior Laravel/PHP developer | Team is growing or replacing someone; codebase exists and is being actively maintained | LinkedIn job posts, company careers page, jobs on the company website | `site:linkedin.com/jobs "senior laravel developer"` |
| Hiring a "Lead Developer" or "Engineering Manager" | Team is scaling beyond the founder; process and architecture decisions are being made | LinkedIn, job boards | `"lead developer" OR "engineering manager" laravel` |
| Hiring for DevOps / SRE / Platform Engineer | Infrastructure is becoming a bottleneck; they need someone to stabilize deployments, queues, or cloud costs | LinkedIn, job boards | `"devops engineer" OR "platform engineer" laravel` |
| Hiring a QA / Test Engineer | Testing is a known gap; coverage is low; they want to improve it | LinkedIn, job boards | `"test engineer" OR "QA engineer" php laravel` |
| Hiring a freelance/contract Laravel developer (not FTE) | They need short-term help — the ideal entry point for a productized audit or sprint | Upwork, freelance platforms, LinkedIn contract posts | `"contract" OR "freelance" laravel developer` |
| Replacing a developer who left | Knowledge drain; someone familiar with the codebase is gone | LinkedIn — watch for "looking for new opportunities" posts from devs at companies in your ICP | Monitor former employees' LinkedIn activity |

**How to act on it:** "Noticed you're hiring a senior Laravel developer — if legacy code or test coverage is slowing down your onboarding, I can run a 5-day codebase audit and give you a prioritized fix plan."

---

## Signal type 2: Tech stack mentions

A company publicly mentioning their stack reveals what they work with and often implies what they struggle with.

| Signal | What it tells you | Where to find it | Search example |
|---|---|---|---|
| Job description mentions Laravel, Livewire, Inertia, Vue | Confirms the stack; tells you what version and patterns they use | LinkedIn job posts, company careers page | `"laravel" AND ("livewire" OR "inertia" OR "vue")` |
| Tech blog post or engineering blog mentioning Laravel | Team writes publicly; likely has opinions and pain points | Company blog, engineering blog, Dev.to, Medium | `site:medium.com "laravel" "our team"` |
| GitHub repos or open-source projects using Laravel | The company builds with Laravel publicly; you can inspect their code quality | GitHub, GitHub topics | `github.com topic:laravel` then filter by organization |
| Stack Overflow or forum questions from the company's domain | Someone at the company is publicly asking about a specific problem | Stack Overflow, Laravel.io forums, Reddit r/laravel | Search for the company name + "laravel" on these platforms |
| Company uses Laravel Forge / Vapor / Cloud | They are invested in the Laravel ecosystem; likely have deployment and infra opinions | Laravel Forge/Vapor public lists, BuiltWith, Wappalyzer | BuiltWith.com lookup of company domain |
| Company mentions migrating FROM PHP to another stack | High-stakes migration in progress; they need help deciding or executing | Engineering blog posts, LinkedIn posts, conference talks | `"migrating from PHP" OR "moving away from laravel"` |

**How to act on it:** "Saw your engineering post about using Livewire — if you're running into performance or testing gaps as the team scales, I can do a focused review."

---

## Signal type 3: Incident, performance, and stability pain

When things break or slow down, urgency is highest. These signals indicate active pain.

| Signal | What it tells you | Where to find it | Search example |
|---|---|---|---|
| Status page incidents (slow responses, outages) | Production systems under stress; may need infra or queue review | statuspage.io, company status pages | Check company status pages directly |
| Job post mentioning "scale", "performance", "high traffic" | They are hitting scaling limits; performance is a known concern | LinkedIn job posts | `"laravel" AND ("scale" OR "performance" OR "high traffic")` |
| Engineering blog post about a post-mortem or incident | They had a real outage; they are reflecting on root causes | Company engineering blog | `"post-mortem" OR "incident" laravel site:medium.com` |
| Developer at the company complaining on social media | Direct expression of pain; high signal | X/Twitter, LinkedIn, Reddit | Search company name + "laravel" on X/Twitter |
| Slow page load or performance complaints in reviews | User-facing performance issues | G2, Capterra, Trustpilot reviews | Search company name on review sites |

**How to act on it:** "Noticed your team has been scaling — if queue processing or response times are becoming a bottleneck, I can run a performance audit and identify the top 3 fixes in under a week."

---

## Signal type 4: Migration, refactor, and modernization

Companies actively modernizing old code are prime candidates for audits and sprints.

| Signal | What it tells you | Where to find it | Search example |
|---|---|---|---|
| Job post mentioning "legacy", "refactor", "modernization" | They know they have technical debt and are trying to fix it | LinkedIn job posts | `"laravel" AND ("legacy" OR "refactor" OR "modernization")` |
| Engineering blog post about migrating to a new version (e.g. Laravel 10 → 11) | Active upgrade in progress; may need help | Company blog, Dev.to | `"upgrading to laravel" OR "migrating to laravel 11"` |
| Company hiring for a specific migration project | Migration is scoped as a project; budget exists | LinkedIn, Upwork | `"migration" laravel developer contract` |
| GitHub activity showing large refactors | The team is actively restructuring; you can see what they're doing | GitHub — watch company org repos | Monitor repos for large PRs or directory restructures |
| Conference talk by a company engineer about migration | They have a story to tell; likely still have ongoing migration work | Conference schedules, YouTube | Search conference talk titles |

**How to act on it:** "Saw your team is upgrading to Laravel 11 — if you're hitting breaking changes or test coverage gaps during the upgrade, I can run a focused sprint to unblock it."

---

## Signal type 5: Funding, growth, and scaling events

Companies that just raised money or are scaling fast have budget and urgency.

| Signal | What it tells you | Where to find it | Search example |
|---|---|---|---|
| Just closed a funding round (Seed, Series A, B) | They have fresh budget; engineering team will grow; architecture decisions are being made | Crunchbase, TechCrunch, LinkedIn announcements | Check Crunchbase for recent rounds |
| Company is scaling rapidly (hiring 5+ roles simultaneously) | Growth pressure on systems and processes | LinkedIn — multiple job posts from same company | Track companies posting 5+ eng roles |
| Product launch or major feature release | New features = new code = new potential debt; may need review | Company blog, Product Hunt, LinkedIn | Monitor company LinkedIn for launch posts |
| Company acquired or merged | Codebases being integrated; migration and audit needs are high | TechCrunch, LinkedIn | `"acquired" OR "merger" saas laravel` |

**How to act on it:** "Congrats on the Series A — if scaling your Laravel infrastructure is on the roadmap, I can help you identify the top 3 risks before they become incidents."

---

## Signal type 6: AI adoption interest

Companies exploring or adopting AI tools are actively looking for guidance.

| Signal | What it tells you | Where to find it | Search example |
|---|---|---|---|
| Job post mentioning "AI", "Copilot", "LLM", "AI-assisted" | Team is exploring AI tooling; may need help with workflows | LinkedIn job posts | `"laravel" AND ("AI" OR "copilot" OR "LLM")` |
| Engineering blog post about AI experiments | Team is testing AI; has questions about quality and reliability | Company blog, Dev.to | `"AI" "laravel" site:medium.com` |
| Developer at company posting about AI tools on social media | Individual interest; may be a champion inside the team | X/Twitter, LinkedIn | Search company name + "AI" on X/Twitter |
| Company using AI testing or documentation tools | They are investing in AI-assisted dev; may need help validating results | GitHub repos, tool usage | Check repos for AI-generated commits or tool configs |

**How to act on it:** "Saw your team is exploring AI-assisted development — I've been running experiments on exactly this with Laravel codebases and can show you what actually works vs. what creates more work."

---

## Signal type 7: Agency and consulting overload

Agencies and dev shops that are overloaded are great buyers for subcontracted audits and sprints.

| Signal | What it tells you | Where to find it | Search example |
|---|---|---|---|
| Agency hiring multiple developers at once | Overloaded with client work; may need overflow help | LinkedIn, agency careers pages | `"agency" OR "dev shop" "hiring" laravel` |
| Agency owner posting about being busy or behind | Direct signal of capacity problems | LinkedIn, X/Twitter | Monitor agency owners' posts |
| Agency taking on new client types or technologies | Stretching beyond their core expertise; may need a specialist | LinkedIn posts, agency blog | `"new client" OR "expanding" agency laravel` |

**How to act on it:** "Noticed your agency is scaling up — if you're taking on Laravel projects and need an extra pair of hands for code audits or test coverage sprints, I can deliver those as fixed-scope packages."

---

## How to use signals in your workflow

1. Pick one signal type to focus on per research session (e.g. "hiring signals only" for one day).
2. Find 10 prospects with that signal.
3. Copy the exact signal wording into `TRACKING_SHEET.csv`.
4. Use the signal as the first line of your outreach message.
5. Track which signal types produce the highest reply rate — double down on what works.

## The 30-prospect rule

If you cannot find 30 prospects with visible buying signals in 2 hours of research, your ICP is too narrow or too hard to reach. Broaden the signal type or the buyer group before continuing.
