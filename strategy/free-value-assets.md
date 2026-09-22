# Free Value-First Assets — your "jab" before the "right hook"

You don't ask for a meeting cold. You give value first. This is the jab (Gary V) and the lead magnet (Hormozi). The goal is to make the prospect think "this person already helped me" before you ask for anything.

---

## Rule: give before you ask

Every first contact should include something useful. Not "can I have 15 minutes of your time?" — but "I noticed X, here's a quick thing that might help."

## Before creating new content: use your existing assets

You already have content that proves your expertise. Before creating anything new, use these:

| Existing content | How to use it |
|---|---|
| Laravel 11 migration post (25-30% less boilerplate, 40% faster queries) | Send to prospects upgrading Laravel: "Saw you're on Laravel 10 — here's what I found migrating to 11" |
| PHP 8.4 performance post | Send to prospects with performance pain: "Here's what PHP 8.4 could do for your app" |
| AI agents in Laravel post | Send to prospects exploring AI: "Here's how I'd add AI agents to a Laravel app" |
| Security / container hardening posts | Send to prospects with security concerns |
| CI/CD content | Send to prospects with deployment pain |

---

## The 5 free assets (pick one per prospect)

### 1. Laravel Codebase Risk Checklist (written)
A 1-page checklist of the 10 most common risks in a Laravel codebase. You can send this to anyone, anytime.

**How to use it:** Send as a PDF or link in a LinkedIn message. "I put together a checklist of the 10 Laravel risks I see most often. Thought it might be useful — want me to send it over?"

**What it looks like:**
- [ ] Outdated dependencies (run `composer outdated`)
- [ ] Known security vulnerabilities (run `composer audit`)
- [ ] No automated tests / low test coverage
- [ ] Fat controllers (business logic in controllers, not services)
- [ ] N+1 query problems (lazy loading in loops)
- [ ] No database foreign key constraints
- [ ] Missing indexes on frequently queried columns
- [ ] Hardcoded credentials or debug mode in production config
- [ ] No CI/CD pipeline
- [ ] No error monitoring (Sentry, etc.)

### 2. 5-Minute Loom Teardown (video)
Record a 5-minute Loom video looking at something public about their company — their job posts, their engineering blog, their GitHub repos. Point out one useful observation.

**How to use it:** "I saw you're hiring a Laravel developer — I took 5 minutes to look at what you might want to check before onboarding someone new. Here's a quick video: [Loom link]"

**Script:** "Hey [First name], I saw you're hiring a Laravel dev. Before you bring someone on, there are 3 things worth checking in your codebase so onboarding goes smooth. Let me show you... [screen share: show the checklist, point at the relevant items]. If any of these ring a bell, I can do a deeper audit. No pressure."

### 3. Top 3 Risks from Their Public Repo
If the company has a public GitHub repo, clone it and spend 15 minutes looking at it. Find 3 specific things. Send a short message.

**How to use it:** "I cloned your open-source repo and spent 15 minutes looking at it. Three things stood out: 1) [specific thing with file/line], 2) [specific thing], 3) [specific thing]. Want me to write these up as a quick risk report?"

### 4. Job Post Teardown
When you see a company hiring a Laravel dev, read the job post carefully. It tells you what they're struggling with. Send a message that shows you understand their situation.

**How to use it:** "I read your job post for a senior Laravel developer — sounds like you're dealing with [specific thing from the post]. Before you hire, it might be worth checking [specific risk]. I have a checklist for this — want me to send it?"

### 5. LinkedIn Comment / Reply (Gary V style)
Don't DM cold. Engage with their content first. Reply to their LinkedIn posts with something genuinely useful. Then, after 2–3 interactions, send a DM.

**How to use it:** Comment on their post with a useful observation or tip. Do this 2–3 times over a week. Then: "Hey [First], enjoyed your posts about [topic]. I work with Laravel teams on [specific thing]. If you ever want a quick codebase audit, happy to do one — no strings."

---

## Which asset to use when

| Signal you found | Best free asset |
|---|---|
| Hiring a Laravel developer | Job post teardown or Loom teardown |
| Public GitHub repo | Top 3 risks from their repo |
| Engineering blog post | Reply to the post, then DM with checklist |
| Legacy code / technical debt mention | Risk checklist |
| Performance / scaling mention | Loom teardown or checklist |
| Agency overload | Offer a free mini-audit of one of their client projects |

---

## How this fits in the flow

```
Find signal → Send free value asset → They reply "thanks" → 
Offer the entry audit (€750-1,500) → If yes, deliver audit → 
Offer implementation (€2,500-6,000) → Offer retainer (€1,500-3,500/mo)
```

The free asset is Step 0. It goes BEFORE the outreach messages in START_HERE.
