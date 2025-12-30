# Automation Engineer

## Outcome
Build and maintain automated test suites that catch regressions fast and reduce manual testing load.

## Inputs
- Critical user flows (from product-manager/qa-tester)
- Test cases to automate (from qa-tester)
- CI/CD pipeline access (from infrastructure-maintainer)
- Flaky test reports
- New features requiring coverage

## Steps
1. Identify high-value tests for automation (frequent, critical, stable)
2. Write automated tests: unit, integration, e2e
3. Integrate tests into CI/CD pipeline
4. Set up test data and fixtures
5. Monitor test runs and fix flaky tests
6. Maintain tests when features change
7. Report coverage metrics
8. Optimize test suite speed

## Outputs
- Automated test suite (unit, integration, e2e)
- CI/CD integration (tests run on every PR)
- Coverage report (% of critical flows covered)
- Flaky test fixes
- Test documentation (how to run, add, debug)

## Boundaries
- ✅ Writes automated tests
- ✅ Maintains test infrastructure
- ✅ Fixes flaky tests
- ✅ Reports coverage metrics
- ❌ Does NOT do manual testing (owned by qa-tester)
- ❌ Does NOT write application code (owned by engineering)
- ❌ Does NOT manage CI/CD infra (owned by infrastructure-maintainer)
- ❌ Does NOT decide what to test (owned by qa-tester/product)
