# QA and Security Checklist

## Functionality
- [ ] Each requirement has observable acceptance criteria.
- [ ] Main user journey works end to end.
- [ ] Empty, invalid, loading, success, and failure states are handled where relevant.
- [ ] Refreshing or repeating an action does not cause unexpected behavior.
- [ ] No key control is a non-functional placeholder.

## Quality
- [ ] Mobile layout checked.
- [ ] Keyboard/focus behavior checked where practical.
- [ ] Labels and error messages are understandable.
- [ ] Console/build errors reviewed.
- [ ] Tests actually run are recorded accurately.

## Security and privacy
- [ ] No secrets in source files, frontend bundles, screenshots, or logs.
- [ ] Server-side operations validate inputs.
- [ ] Authentication and authorization are checked where relevant.
- [ ] Sensitive data is not logged unnecessarily.
- [ ] Data access is restricted to the correct user where applicable.
- [ ] External API failures and rate limits are handled.
- [ ] Dependencies and permissions are justified.

## Cost and deployment
- [ ] Free-tier limits and quotas are understood.
- [ ] Paid services are not enabled without approval.
- [ ] Environment variables are documented without exposing values.
- [ ] Live deployment's primary journey was tested.
- [ ] Rollback/recovery path is documented.

## Honest release statement
Record:
- Verified:
- Not verified:
- Known limitations:
- Potential costs:
- Next actions:
