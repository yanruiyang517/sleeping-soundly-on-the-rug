\# Bounty Safety Checklist for Beginners



\## Purpose



This checklist helps beginners evaluate GitHub bounty issues before spending time on them. It focuses on safety, scope control, payment uncertainty, and common scam patterns.



This is not financial advice, investment advice, legal advice, or a guarantee that any bounty will be paid.



\## Quick Evaluation Checklist



Before working on a bounty, check the following items:



| Area                  | What to check                                                                                         | Safer action                                                        |

| --------------------- | ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------- |

| Issue clarity         | The issue has clear requirements, acceptance criteria, and expected deliverables.                     | Avoid vague issues unless the maintainer clarifies the scope.       |

| Existing work         | Search open pull requests and comments for duplicate attempts.                                        | Do not start if several PRs already solve the same issue.           |

| Repository activity   | Check recent commits, maintainer responses, and issue activity.                                       | Prefer active repositories with recent maintainer feedback.         |

| Payment terms         | Check whether the bounty amount, payout method, and eligibility rules are written clearly.            | Treat unclear payout terms as uncertain.                            |

| Secrets and keys      | The task should not require private keys, seed phrases, API keys, cookies, or production credentials. | Refuse tasks asking for secrets or private account access.          |

| Upfront payment       | The requester should not ask you to pay a fee, buy a token, or deposit money before working.          | Treat upfront payment requests as a scam signal.                    |

| Off-platform pressure | Be careful if someone pushes you to Telegram, Discord, WhatsApp, or email for payment details.        | Keep technical discussion and deliverables on GitHub when possible. |

| Scope size            | The work should be small enough to complete and test.                                                 | Timebox beginner bounties and avoid large rewrites.                 |



\## Common Scam or High-Risk Patterns



\### 1. “Pay first to unlock the bounty ?



A requester says the bounty is real but asks you to pay a registration fee, gas fee, verification fee, or token purchase first.



Safer response: do not pay. Legitimate open-source contribution work should not require contributors to send money before contributing.



\### 2. “Use this seed phrase or private key ?



A task asks you to use, generate, paste, or submit wallet seed phrases, private keys, browser cookies, or cloud credentials.



Safer response: refuse the task. Real development work should use test credentials, mock data, or documented local setup.



\### 3. “Guaranteed payout if you do this quickly ?



A requester promises a guaranteed reward without clear acceptance criteria, escrow, maintainer approval, or public issue history.



Safer response: treat the payout as uncertain until the rules are visible and verifiable.



\### 4. “Large project, tiny bounty, unclear scope ?



The issue asks for a full product, large refactor, production deployment, or complex integration, but gives only a small or unclear bounty.



Safer response: ask for a smaller scoped task or skip it.



\### 5. “Duplicate PR race ?



The issue is simple, but many pull requests already exist.



Safer response: check existing PRs first. If multiple PRs already solve it, the chance of acceptance is low.



\## Beginner-Friendly Bounty Workflow



\### Step 1: Read the issue carefully



Check:



\* What exactly needs to change

\* Which files are likely involved

\* Whether acceptance criteria are written

\* Whether the issue references another issue, bounty page, or sponsor instruction

\* Whether payout rules are public



\### Step 2: Check for duplicate work



Use GitHub search or GitHub CLI:



```bash

gh pr list --repo OWNER/REPO --search "ISSUE\_NUMBER"

```



Also read recent comments. If someone already posted an attempt, compare whether the issue is still open and whether maintainers asked for revisions.



\### Step 3: Estimate the work



Prefer tasks that are:



\* Documentation improvements

\* Small bug fixes

\* Test additions

\* Simple frontend changes

\* Configuration fixes

\* Clear template updates



Avoid tasks that require:



\* Production secrets

\* Paid services

\* Private customer data

\* Large architecture changes

\* Unclear external API access

\* Financial or token promotion claims



\### Step 4: Make a small change



Keep the pull request focused. Do not rewrite unrelated files. Do not add large dependencies unless the issue requires them.



\### Step 5: Submit with evidence



A good bounty submission should include:



\* What changed

\* Why it helps

\* How it was tested

\* Screenshots or command output when relevant

\* The related issue number

\* Remaining caveats



\## Notes on Bounty Platforms



Different platforms handle payment, review, and eligibility differently. A platform being reputable does not guarantee that every issue will pay out.



Useful places to review before working:



\* GitHub issue and pull request history

\* The repository's README and CONTRIBUTING files

\* The bounty platform's current terms and payout rules

\* Maintainer comments on the specific issue



Examples of platforms or ecosystems contributors may encounter include GitHub Issues, Algora, Gitcoin, OnlyDust, and Code4rena. Always verify the current rules directly on the relevant platform before relying on a bounty.



\## Submission Template



```markdown

\## Summary



Briefly describe what you changed and which issue it addresses.



\## Changes



\- Added or updated:

\- Clarified:

\- Removed or avoided:



\## Testing



\- Ran:

\- Checked:

\- Not run, because:



\## Safety / Secrets Check



\- \[ ] No seed phrases

\- \[ ] No private keys

\- \[ ] No API keys

\- \[ ] No client-private data

\- \[ ] No investment promises

\- \[ ] No production credentials



\## Caveats



Explain what could still be wrong, incomplete, or dependent on maintainer review.



\## Related Issue



Closes #ISSUE\_NUMBER

```



\## What Could Still Be Wrong



\* Bounty rules can change after this checklist is written.

\* A maintainer may choose another PR even if your work is correct.

\* A bounty may require KYC, regional eligibility, or platform-specific payout steps.

\* Public issue descriptions may be incomplete.

\* This checklist reduces risk but cannot remove all risk.

## References and Receipts

These references are starting points for checking bounty rules, platform terms, and submission expectations. Contributors should always verify the current rules on the relevant platform before relying on a bounty.

* GitHub Docs — Issues and pull requests: https://docs.github.com/en/issues
* GitHub Docs — Keeping your account and data secure: https://docs.github.com/en/authentication/keeping-your-account-and-data-secure
* Algora Docs — Bounties and contributor rewards: https://algora.io/docs
* Algora Bounties — GitHub bounty workflow examples: https://algora.io/bounties/
* Gitcoin — Bounties as a task-based funding mechanism: https://gitcoin.co/mechanisms/bounties
* Code4rena Docs — Submission guidelines: https://docs.code4rena.com/competitions/submission-guidelines
* OnlyDust — Historical/open-source funding context; verify current availability before relying on it: https://www.onlydust.com/



