# Feature Workflow: Idea to Verified Change

## 1. Define
Write a short problem statement and observable acceptance criteria. Separate must-have requirements from nice-to-haves.

## 2. Inspect
Read relevant files and existing patterns. Identify dependencies and avoid duplicating existing functionality.

## 3. Plan
Describe the smallest implementation, affected files, failure states, and verification steps. Ask for clarification when ambiguity affects security, cost, architecture, or user data.

## 4. Implement one stage
Give the AI builder only the current stage. Tell it to preserve unrelated behavior and summarize every file changed.

## 5. Review
Check the diff or generated files. Look for:
- Unrelated edits
- Missing loading/empty/error states
- Hard-coded secrets
- Unsafe input handling
- Broken responsive layout/accessibility
- Dependencies added without justification
- Fake or placeholder functionality presented as real

## 6. Verify
Run relevant build, lint, type-check, unit, integration, and manual checks where available. Record what was actually run. If the environment cannot run a check, mark it as not run.

## 7. Checkpoint
Create a small commit or other recoverable checkpoint once the change is understood and verified to the extent possible.

## 8. Report
Summarize behavior, files, verification evidence, known limitations, and next steps.

## Stop conditions
Pause before proceeding if:
- The task would expose credentials or personal data.
- A change could delete or irreversibly alter data.
- A paid service or plan is required.
- Requirements conflict.
- The requested feature depends on an unverified external API capability.
