# Release and Deployment Workflow

## Before deployment

1. Confirm the target branch and the exact commit to deploy.
2. Confirm all required environment variables are documented.
3. Ensure real secrets are stored in the hosting provider's secret manager, not in frontend code or GitHub files.
4. Run available build and test commands.
5. Review authentication, authorization, user data handling, and API endpoints.
6. Check responsive behavior and the primary user journey.
7. Confirm external services, quotas, and potential costs.
8. Document known limitations.

## Deploy

1. Deploy the verified commit through the selected hosting provider.
2. Record the deployment URL and commit/version identifier.
3. Do not enable paid resources without approval.
4. Avoid exposing preview deployments containing sensitive test data.

## Smoke test the live application

- [ ] Application loads.
- [ ] Primary user journey works.
- [ ] Loading and error states behave correctly.
- [ ] Backend/API calls succeed or fail clearly.
- [ ] Secrets are not visible in client code or browser network responses.
- [ ] Mobile layout is usable.
- [ ] No unexpected paid resource has been enabled.

## After deployment

- Record what was verified and what was not.
- Record known issues and a rollback procedure.
- Keep the previous working version available where possible.
- Do not call the release fully verified if only the landing page was checked.
