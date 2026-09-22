# Offer: AI-Assisted Test Coverage Sprint

## Who it's for

A technical founder, CTO, or engineering manager at a company (1–50 people) that has a Laravel/PHP codebase with low or no automated tests, and wants to add coverage quickly using AI-assisted tools — but isn't sure if AI-generated tests are reliable or how to validate them.

## What pain it solves

- "We have no tests and every deploy feels like a gamble."
- "We want to add tests but it keeps getting deprioritized."
- "We tried using AI to generate tests but we don't know if they're actually any good."
- "Our test coverage is 10% and we need to get to 60%+ before we can refactor safely."

## Observable buying signals

- Job post mentioning "testing" or "QA" alongside Laravel
- Developer at the company posting about test coverage or CI issues
- Company adopting AI tools (Copilot, Claude, etc.) and unsure about quality
- Engineering blog post about reliability or deployment confidence
- Company about to do a major refactor or migration (needs test coverage first)

## What the client gets

1. A test coverage assessment (current state: what % is covered, what's critical and uncovered)
2. A batch of AI-generated tests for the most critical code paths (controllers, services, models)
3. Human-reviewed and validated test quality report (which AI tests are good, which need fixing, which to throw away)
4. A CI integration plan so tests run automatically on every PR
5. A one-page "testing playbook" so the team can continue adding AI-assisted tests after you leave
6. A 60-minute walkthrough call with the team

## What you actually do (delivery methodology)

### Day 1: Baseline assessment
1. Get read access to the codebase
2. Run the existing test suite: `php artisan test` or `vendor/bin/phpunit`
3. Generate a coverage report: `php artisan test --coverage` (requires Xdebug or PCOV)
4. Identify the 5–10 most critical code paths (controllers with the most traffic, services with the most business logic, models with the most relationships)
5. Document the current coverage percentage and where the gaps are

### Day 2: AI test generation setup
1. Choose the AI tool(s) you'll use: GitHub Copilot, Claude, or GPT-4 — or a combination
2. For each critical code path:
   - Feed the source file to the AI tool
   - Ask it to generate unit tests and feature tests
   - Prompt example: "Generate PHPUnit feature tests for this controller. Cover the happy path, validation errors, and edge cases. Use Laravel's testing factories."
3. Save the generated tests to the appropriate test directories

### Day 3: Human review and validation
1. Run all AI-generated tests: which ones pass, which fail?
2. For failing tests:
   - Is the test wrong (AI misunderstood the logic)? Fix or discard.
   - Is the code wrong (the test found a real bug)? Report it — this is gold for the client.
3. For passing tests:
   - Is the test actually testing something meaningful, or is it trivial (e.g. `assertTrue(true)`)?
   - Does it test the right behavior?
4. Remove or rewrite tests that are meaningless or misleading
5. Document which AI tools produced the best results (this is valuable data for the client and for your content)

### Day 4: CI integration
1. Add the test suite to the CI pipeline (GitHub Actions, GitLab CI, etc.)
2. Create a simple GitHub Actions workflow that runs tests on every PR:
   ```yaml
   name: Tests
   on: [pull_request]
   jobs:
     tests:
       runs-on: ubuntu-latest
       steps:
         - uses: actions/checkout@v4
         - uses: shivammathur/setup-php@v2
           with:
             php-version: '8.3'
         - run: composer install --no-interaction --prefer-dist
         - run: php artisan test
   ```
3. Test that it works by creating a test PR
4. Document the workflow so the team can maintain it

### Day 5: Playbook and walkthrough
1. Write the "testing playbook" — a one-page guide for the team:
   - How to generate AI tests (which tool, which prompt)
   - How to validate them (the review checklist from Day 3)
   - How to add them to CI
   - What to test first (critical paths) vs. later (nice-to-have)
2. Schedule the 60-minute walkthrough call
3. Deliver all artifacts: tests, coverage report, playbook, CI config

## Required access and tools

- Read and write access to the codebase (you'll be adding test files)
- Access to an AI tool: GitHub Copilot, Claude (web or API), or GPT-4
- Local PHP/Laravel environment with Xdebug or PCOV for coverage
- GitHub Actions or equivalent CI access

## Skills you need

- Writing PHPUnit tests in Laravel (you know this)
- Using AI coding tools (Copilot, Claude, GPT-4) — you've been experimenting with these
- GitHub Actions or CI configuration (you've done CI/CD)
- Critical evaluation of AI-generated code (knowing when AI is wrong — this is your strength)

## Can I deliver this? Self-assessment checklist

- [ ] I can write PHPUnit feature and unit tests for Laravel
- [ ] I can generate test coverage reports
- [ ] I have used at least one AI tool (Copilot, Claude, GPT-4) to generate code
- [ ] I can critically evaluate whether AI-generated tests are meaningful
- [ ] I can set up a basic GitHub Actions workflow for PHP tests
- [ ] I can explain to a team why some AI tests are good and others need fixing
- [ ] I can do this in 5 working days or less

If you check 5+ boxes, you can deliver this offer.

## Delivery risk level: MEDIUM

You are adding files to their codebase (test files), which is higher risk than a read-only audit. Mitigate by:
- Working in a separate branch
- Never modifying existing application code (only adding test files)
- Having the team review and merge your branch themselves

## Suggested starter price range

€750–2,000 for the full sprint (assessment + AI-generated tests + review + CI setup + playbook + walkthrough).

- €750 for a small codebase (focus on 3–5 critical paths)
- €1,200 for a medium codebase (5–10 critical paths)
- €2,000 for a large codebase (10+ critical paths, full CI setup)

## What proof/content can come from it

- A YouTube video: "I let AI write tests for a real Laravel app — here's what happened" (show the good, bad, and surprising)
- A LinkedIn post: "AI-generated tests: 40% were useless, 20% found real bugs. Here's how to tell the difference."
- A case study: before/after coverage percentages
- A reusable "AI testing playbook" as a lead magnet

## When NOT to sell this offer

- The codebase is too small (less than 5 controllers/services — tests won't take a full week)
- The team already has 60%+ test coverage (they don't need a sprint, they need maintenance)
- The client has no CI/CD and refuses to set one up (tests without CI are less valuable)
- You haven't used AI tools enough to evaluate their output critically
