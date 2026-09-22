# Step 1 — Pick who you sell to

You have never picked an ICP before. This guide takes you from "I don't know who to sell to" to "I have one buyer group chosen" in under an hour.

You are not picking forever. You are picking for a 30-day test. If it doesn't work, you pick again.

**Quick steps:**
1. Read the "Should you sell to CTOs?" table below
2. Score the 5 candidate buyer groups on 8 criteria
3. Pick the highest-scoring one
4. Write your one-line ICP at the bottom of this file
5. Then go to `02-validate-market.md`

---

## What an ICP actually is

An ICP is not "companies that use Laravel." That's a market. An ICP is a specific person, at a specific type of company, who has a specific pain they will pay to solve right now.

An ICP answers four questions:
1. **Who** is the buyer? (role: founder, CTO, head of engineering, agency owner, technical lead)
2. **Where** do they work? (company type: SaaS, agency, startup, e-commerce, enterprise)
3. **What** pain do they have? (legacy code, scaling, testing, cloud costs, AI adoption)
4. **Why now?** (what event or trigger makes this urgent — see `BUYING_SIGNALS.md`)

---

## Step 2: Should you sell to CTOs?

Short answer: sell to the person who owns both the technical pain AND the budget. That is not always the CTO.

| Company size | Who owns the pain + budget | How to reach them |
|---|---|---|
| Solo founder / pre-seed (1–5 people) | Founder / technical co-founder | LinkedIn, X/Twitter, indie hacker communities |
| Seed / Series A (5–30 people) | CTO / VP Engineering / Head of Engineering | LinkedIn, engineering blog, conference talks |
| Series B+ / mid-market (30–200 people) | Engineering Manager / Platform Lead / Staff Engineer | LinkedIn, harder to reach directly, may need warm intro |
| Agency / dev shop (5–50 people) | Agency owner / Technical Director / Delivery Lead | LinkedIn, agency directories, referrals |
| Enterprise (200+ people) | Multiple stakeholders, long sales cycles, procurement | Not recommended for your first ICP |

**Rule of thumb:** If the company has fewer than 30 people, the CTO or founder is accessible and is your buyer. If the company has 30–200 people, the CTO exists but is hard to reach — target the Engineering Manager or Technical Lead instead. If the company has 200+ people, the sales cycle is too long for a first ICP.

**Do not default to "CTO" unless the company is small enough that the CTO is one LinkedIn message away.**

---

## Step 3: List your candidate buyer groups

Below are 5 candidate buyer groups based on your expertise (Laravel/PHP, Docker/K8s, AI-assisted dev, queue systems, infrastructure). These are not the only options — they are starting points. Pick 3–5 to score.

### Candidate buyer groups

**A. Technical founder of a Laravel SaaS (1–10 people)**
- Who: Founder / technical co-founder
- Pain: Shipping fast but accumulating debt; infrastructure decisions piling up; no senior reviewer
- Why you: You've been the senior dev who cleans up exactly this
- Reachability: High — founders are on LinkedIn and X/Twitter daily
- Budget: Limited but decisive — they can say yes in one call

**B. CTO / Head of Engineering at a growing Laravel SaaS (10–50 people)**
- Who: CTO, VP Engineering, Head of Engineering
- Pain: Team is scaling; codebase is getting complex; needs architecture review or infra help
- Why you: Deep Laravel + infra experience; can audit and recommend
- Reachability: Medium — findable on LinkedIn, may need warm intro
- Budget: Good — they have engineering budget and authority

**C. Agency owner / Technical Director at a dev shop (5–50 people)**
- Who: Agency owner, Technical Director, Delivery Lead
- Pain: Overloaded with client work; needs overflow capacity for audits, sprints, or specialized work
- Why you: You can deliver fixed-scope packages they can white-label or resell
- Reachability: High — agency owners are very active on LinkedIn
- Budget: Good — they bill clients and can mark up your work

**D. Engineering Manager at a mid-market company with legacy PHP (30–200 people)**
- Who: Engineering Manager, Platform Lead, Staff Engineer
- Pain: Legacy codebase is slowing the team; migration is on the roadmap; testing is a gap
- Why you: Legacy modernization + AI-assisted dev is your strength
- Reachability: Low–Medium — harder to reach, may need warm intro or referral
- Budget: Strong — enterprise budgets, but slow decision-making

**E. Solo developer / indie hacker building a Laravel product**
- Who: Solo developer, indie hacker, solo founder
- Pain: Stuck on architecture, infra, or deployment; needs a second pair of eyes
- Why you: You've built and shipped products; you can review and unblock fast
- Reachability: High — active on X/Twitter, indie hacker communities
- Budget: Low — may not be able to pay much; good for case studies and testimonials, not revenue

---

## Step 4: Score each candidate buyer group

Copy this table. Score each buyer group from 1 (weak) to 5 (strong) on each criterion. Then add up the scores.

| Criterion | A. Tech founder (SaaS) | B. CTO (growing SaaS) | C. Agency owner | D. Eng manager (legacy) | E. Solo dev / indie |
|---|---|---|---|---|---|
| Pain urgency (how much does this hurt right now?) | | | | | |
| Ability to pay (do they have budget?) | | | | | |
| Your credibility (can they tell you know what you're talking about?) | | | | | |
| Ease of reaching them (can you find and message them on LinkedIn?) | | | | | |
| Visible buying signals (can you find 30+ prospects with signals in 2 hours?) | | | | | |
| Delivery confidence (do you know how to deliver the fix?) | | | | | |
| Speed to first result (how fast can you get a meeting booked?) | | | | | |
| YouTube / content alignment (will your content reach this buyer?) | | | | | |
| **Total (max 40)** | | | | | |

### What the scores mean

- **30–40:** Strong candidate. Pick this for your 30-day sprint.
- **20–29:** Possible, but has a weakness. Note the weak criterion and decide if you can work around it.
- **Below 20:** Skip for now. Too hard to reach, too slow, or too low-budget.

---

## Step 5: Validate with the 30-prospect test

Before committing to your chosen buyer group, run this test:

1. Open LinkedIn (or your preferred source).
2. Search for 30 prospects who match your chosen buyer group AND show a visible buying signal (from `BUYING_SIGNALS.md`).
3. Time yourself. If it takes less than 2 hours, the ICP is viable.
4. If you cannot find 30 prospects with signals in 2 hours, the ICP is too narrow or too hard to reach. Pick your second-highest scoring buyer group and repeat.

This is not about messaging them yet. This is about confirming the pool exists and is findable.

---

## Step 6: Write your one-line ICP

Once you've picked a buyer group and passed the 30-prospect test, fill in this template:

```
[Buyer role] at [company type and size] who needs [specific outcome] without [common objection or constraint].
```

Example (filled):
```
Technical founder of a Laravel SaaS (1–10 people) who needs a codebase audit and prioritized fix plan without hiring a senior developer or pausing feature work.
```

---

## Step 7: What comes next

After you pick your ICP:
1. Pick one offer from `strategy/offers/` that matches your chosen buyer group's pain.
2. Adapt the offer to your ICP (we'll help you with this in the next step).
3. Rewrite `business/01-pick-icp.md` with your finalized one-line ICP (fill in the template at the bottom of this file).
4. Start the 30-day validation sprint from `business/03-weekly-workflow.md`.

You are not committing to this ICP forever. You are testing it for 30 days. If it doesn't produce meetings, you come back to this file, pick a different buyer group, and test again.

---

## Quick reference: decision summary

1. Do NOT pick an offer first. Pick a buyer group first.
2. Score 3–5 candidate buyer groups on 8 criteria.
3. Pick the highest-scoring buyer group.
4. Run the 30-prospect test (can you find 30 prospects with signals in 2 hours?).
5. Write your one-line ICP.
6. Then pick an offer that matches that buyer's pain.
