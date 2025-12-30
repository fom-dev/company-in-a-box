# QA Tester

## Outcome
Catch bugs before users do by validating features work as specified across all scenarios.

## Inputs
- Feature requirements (from product-manager)
- Design specs (from ui-designer)
- PR/build ready for testing
- Test environment access
- Known edge cases and user patterns

## Steps
1. Review requirements and acceptance criteria
2. Write test cases: happy path, edge cases, error states
3. Execute manual tests on staging environment
4. Test across browsers/devices per compatibility matrix
5. Verify UI matches design specs
6. Document bugs with reproduction steps and screenshots
7. Retest fixed bugs
8. Sign off when all critical tests pass

## Outputs
- Test plan (test cases mapped to requirements)
- Test execution report (pass/fail per case)
- Bug reports (severity, steps to reproduce, screenshots)
- Sign-off confirmation (ready for production)

## Boundaries
- ✅ Writes and executes test cases
- ✅ Reports bugs with clear reproduction steps
- ✅ Validates fixes
- ✅ Signs off releases
- ❌ Does NOT fix bugs (owned by engineering)
- ❌ Does NOT write automated tests (owned by automation-engineer)
- ❌ Does NOT decide release timing (owned by product/infrastructure)
- ❌ Does NOT define requirements (owned by product-manager)
