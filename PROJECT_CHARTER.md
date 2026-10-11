# Project Charter — AI Development Workflow

## 1. Purpose

Create a reusable, lightweight system for planning, implementing, testing, reviewing, and deploying applications with AI assistance.

## 2. Problem

AI builders can generate code quickly, but projects can become unreliable when requirements are vague, changes are too broad, testing is skipped, or platform limitations and costs are ignored.

## 3. Intended users

Initially: one beginner-to-intermediate builder using an Android phone, ChatGPT, an AI application builder, and GitHub. The workflow should remain useful for future collaborators.

## 4. Goals

- Make project requirements explicit before implementation.
- Break large tasks into small, testable stages.
- Preserve source code and decisions in GitHub.
- Reduce regressions caused by broad AI edits.
- Make testing claims honest and reproducible.
- Surface security risks, platform limits, and possible costs early.
- Keep the workflow tool-agnostic where practical.

## 5. Non-goals for version 0.1

- Building a standalone SaaS product.
- Automating every step without human review.
- Guaranteeing that AI-generated code is correct.
- Replacing professional security, legal, or compliance reviews.
- Depending on paid AI APIs or services.

## 6. Success criteria

The workflow is successful when we can use it to build a small real feature and answer:
- What was requested?
- What changed?
- How was it tested?
- What remains uncertain?
- How can we recover if the change breaks something?

## 7. Constraints

- Start with a ₹0 workflow where possible.
- Primary working device: Android phone.
- GitHub is the source of truth.
- AI builders may be used for implementation, but code ownership and exportability matter.
- Paid services require discussion and explicit approval.

## 8. Risks

| Risk | Mitigation |
|---|---|
| AI changes unrelated code | Limit scope; ask for a change summary; inspect diffs |
| Tests are claimed but not run | Require a test evidence section |
| API keys leak | Use server-side secrets; scan changes before committing |
| Builder lock-in | Sync/export code; document external dependencies |
| Free-tier limits change | Verify current limits before relying on a provider |
| Overengineering | Start with the smallest useful workflow and improve from real use |

## 9. First milestone

Create and review the starter files, then apply them to a small feature in the Web Research Assistant project.
