# Testing Strategy

Good teams do not rely on only one test type. They build a test portfolio.

## Test portfolio

- Unit tests for business logic
- Integration tests for service and DB boundaries
- End-to-end tests for user-critical flows
- Contract tests for API compatibility
- Static checks (types, lint, formatting)

## What to prioritize

- Critical user journeys
- Money movement and irreversible actions
- Auth and permission boundaries
- Data migrations and version compatibility

## Resources

- [Testing Trophy](https://kentcdodds.com/blog/the-testing-trophy-and-testing-classifications)
- [Martin Fowler - Test Pyramid](https://martinfowler.com/articles/practical-test-pyramid.html)
- [Playwright Docs](https://playwright.dev/docs/intro)
- [Jest Docs](https://jestjs.io/docs/getting-started)
- [Pact Contract Testing](https://docs.pact.io/)
