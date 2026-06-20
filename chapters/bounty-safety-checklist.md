# Bounty Safety Checklist for Beginners

## Purpose

This checklist helps beginners evaluate GitHub bounty issues before spending
time on them. It focuses on safety, scope control, payment uncertainty, and
common scam patterns.

This is not financial, investment, or legal advice, and it is not a guarantee
that any bounty will be paid.

## Before You Start

- [ ] **Read the issue:** Confirm that the expected deliverable and acceptance
  criteria are specific enough to test or review.
- [ ] **Check for existing work:** Search open pull requests and recent issue
  comments for duplicate attempts.
- [ ] **Check repository activity:** Look for recent commits and maintainer
  responses before investing significant time.
- [ ] **Verify the bounty terms:** Confirm the amount, payout method,
  eligibility rules, claim process, and who decides acceptance.
- [ ] **Protect secrets:** The work must not require seed phrases, private keys,
  API keys, cookies, production credentials, or client-private data.
- [ ] **Keep your financial floor:** Do not pay a fee, buy a token, or deposit
  money to unlock a bounty.
- [ ] **Keep a public trail:** Prefer public issue and pull request discussion
  for scope, review, and submission evidence.
- [ ] **Timebox the work:** Prefer a change that is small enough to complete,
  test, and explain without a large rewrite.

An unchecked item does not always mean the task is fraudulent. It means there
is uncertainty to resolve before starting.

## Common Scam or High-Risk Patterns

### "Pay first to unlock the bounty"

A requester asks for a registration fee, gas fee, verification fee, token
purchase, or deposit before you can contribute.

**Safer response:** Do not pay. Ask for the full process to be documented on
the public issue or bounty platform. If payment is still required, skip the
task.

### "Use this seed phrase or private key"

A task asks you to paste, generate, or submit wallet recovery words, private
keys, browser cookies, cloud credentials, or production secrets.

**Safer response:** Refuse the task. Legitimate development should use test
credentials, mock data, or a documented local environment. Never post a real
secret in an issue, pull request, screenshot, log, or commit.

### "Guaranteed payout if you do this quickly"

A requester promises a guaranteed reward without clear acceptance criteria,
maintainer approval, escrow, or a public payout process.

**Safer response:** Treat the payout as unconfirmed until the rules and
decision-maker are visible. A correct contribution can still lose to another
submission or fail an eligibility rule.

### "Large project, tiny bounty, unclear scope"

The issue asks for a full product, large refactor, production deployment, or
complex integration while leaving the deliverables or bounty unclear.

**Safer response:** Ask the maintainer to define a smaller acceptance target.
Skip the task if the scope remains open-ended.

### "Duplicate pull request race"

Several pull requests already attempt the same issue, or another contributor
is assigned and actively responding.

**Safer response:** Read the existing attempts before writing code. Continue
only when a maintainer identifies a missing case or invites another approach.

## Beginner-Friendly Bounty Workflow

### Step 1: Read the Issue and Rules

Write down:

- the exact behavior or document that must change,
- the files likely involved,
- the acceptance criteria,
- the bounty amount and payment method,
- any claim, assignment, identity, or regional requirements,
- who has authority to accept the work.

If the issue and the bounty platform disagree, ask for clarification in public
before starting.

### Step 2: Check for Duplicate Work

Read linked pull requests and recent comments. You can also search with the
GitHub CLI:

```bash
gh pr list --repo OWNER/REPO --state all --search "ISSUE_NUMBER"
```

Search by the issue title and relevant function name too; not every pull
request includes the issue number.

### Step 3: Estimate the Work

Beginner-friendly tasks usually have a narrow review surface, such as:

- documentation improvements,
- small bug fixes with a reproducible case,
- tests for existing behavior,
- focused configuration fixes,
- simple user-interface corrections.

Avoid tasks that depend on production secrets, paid services, private customer
data, complex deployment, large architecture changes, or unclear external API
access.

### Step 4: Make the Smallest Complete Change

Keep the pull request focused on the acceptance criteria. Follow the existing
project style, add a regression test for a bug when practical, and do not
rewrite unrelated files or upgrade dependencies without a clear need.

### Step 5: Submit With Receipts

Use the repository's
[bounty submission template](../templates/bounty-submission.md). Include:

- the chapter or issue addressed,
- what changed and why it helps,
- the exact checks or tests run,
- screenshots or links when relevant,
- sources for factual claims,
- remaining limitations or uncertainty,
- a completed secrets check.

Only claim checks you actually ran. If something could not be tested, state
the reason and the alternative review performed.

## Platform Notes

A recognizable bounty platform can document a workflow, but it does not make
every linked issue active, eligible, or guaranteed to pay. Before relying on a
listing:

- read the platform's current contributor and payout rules,
- confirm that the specific bounty is still active,
- check whether claiming or maintainer assignment is required,
- verify payout method and eligibility before doing substantial work,
- keep links or screenshots of the rules that applied when you started.

## What Could Still Be Wrong

- Bounty rules, links, and eligibility requirements can change after this
  checklist is written.
- A maintainer may choose another pull request even if your work is correct.
- A bounty may require identity verification, regional eligibility, tax
  information, or platform-specific payout steps.
- Public issue descriptions may omit constraints that appear during review.
- A repository or platform can be legitimate while a person impersonating it
  is not.
- This checklist reduces avoidable risk but cannot remove all risk or guarantee
  payment.

## References and Receipts

- [GitHub Docs: About issues](https://docs.github.com/en/issues/tracking-your-work-with-issues/about-issues)
- [GitHub Docs: Pull requests](https://docs.github.com/en/pull-requests)
- [GitHub Docs: Keeping your account and data secure](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure)
- [Algora source repository](https://github.com/algora-io/algora)
- [Algora bounties](https://algora.io/bounties)
