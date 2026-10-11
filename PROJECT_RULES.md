# AI-Assisted Project Rules

Use these rules with ChatGPT, Lovable, Bolt, Replit, or another AI coding tool.

## Before editing

1. Read the current project structure and relevant files.
2. Restate the task and acceptance criteria briefly.
3. Identify assumptions, dependencies, and affected areas.
4. Ask before proceeding if a missing decision could change the architecture, data model, cost, or security posture.
5. Prefer the smallest change that satisfies the requirement.

## While editing

1. Preserve working behavior unless the task explicitly changes it.
2. Do not replace entire files or restructure the project unnecessarily.
3. Do not add packages, services, databases, or API providers without explaining why.
4. Never put secrets, private keys, passwords, or privileged tokens in client-side code.
5. Do not fabricate data, successful API responses, test results, or citations.
6. Include loading, empty, error, and success states for user-facing asynchronous operations.
7. Keep accessibility, responsive layout, and understandable error messages in mind.
8. Do not remove existing tests merely to make a build pass.

## After editing

Provide:
- Summary of files changed.
- Behavior implemented.
- Tests/checks actually run and their results.
- Checks not run and why.
- Known limitations, assumptions, and risks.
- Any required manual setup, environment variables, or deployment steps.

## GitHub and release safety

- Keep GitHub as the source of truth.
- Use small commits or branches when the workflow supports them.
- Never commit `.env` files or real credentials.
- Avoid destructive database migrations or data deletion without explicit approval.
- Do not enable paid plans or services without explicit approval.
- Prefer reversible changes and a documented rollback path.

## Communication

Be direct and specific. If a requirement is ambiguous, explain the uncertainty instead of guessing. If a proposed approach is risky or unnecessary, say so and offer a simpler alternative.
