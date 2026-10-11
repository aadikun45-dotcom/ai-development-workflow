# AI Development Workflow

A reusable, practical workflow for building software with AI builders, ChatGPT, and GitHub.

## Why this repository exists

This repository helps turn app ideas into maintainable, testable software without relying blindly on a single AI builder. It contains project rules, planning templates, implementation procedures, and release checklists.

## Core principles

1. **Functionality before polish:** A feature is not done because the UI looks convincing.
2. **Small, verifiable changes:** Build in stages and test each meaningful change.
3. **GitHub is the source of truth:** Preserve code, decisions, and working checkpoints.
4. **No invented verification:** Never claim something was tested unless it was actually run and observed.
5. **Security by default:** Keep secrets out of frontend code, prompts, screenshots, logs, and Git history.
6. **Explicit trade-offs:** State limitations, costs, assumptions, and risks.
7. **User approval for costly or destructive actions:** Do not enable paid services, delete data, or make irreversible changes without approval.
8. **Portable where practical:** Prefer standard code and documented deployment steps over unnecessary platform lock-in.

## Repository map

- `docs/PROJECT_CHARTER.md` — purpose, scope, and success criteria.
- `instructions/PROJECT_RULES.md` — reusable rules for AI-assisted development.
- `templates/PRD_TEMPLATE.md` — product requirements template.
- `templates/IMPLEMENTATION_PLAN.md` — staged implementation plan.
- `templates/BUG_REPORT.md` — reproducible bug-report template.
- `workflows/FEATURE_WORKFLOW.md` — idea-to-tested-feature process.
- `workflows/RELEASE_WORKFLOW.md` — release and deployment process.
- `checklists/QA_SECURITY_CHECKLIST.md` — pre-release quality and security checks.

## How to use it on a new project

1. Copy the PRD template and fill in the problem, users, scope, and acceptance criteria.
2. Write a staged implementation plan before asking an AI builder to make large changes.
3. Give the builder only the current stage and clear acceptance criteria.
4. Inspect the diff or changed files when possible.
5. Run the available checks and record what was and was not tested.
6. Use the QA/security checklist before deploying.
7. Record important decisions and known limitations.

## Definition of done

A feature is done only when:
- Its expected behavior is specified.
- The implementation is present.
- Relevant checks have been run where possible.
- Failures and edge cases have been considered.
- Security-sensitive behavior has been reviewed.
- Remaining limitations are documented.

## Current status

**Version:** 0.1.0  
**Status:** Initial starter framework; not yet validated against a real project.  
**Next milestone:** Apply this workflow to a small feature, record friction points, and revise the templates based on evidence.
