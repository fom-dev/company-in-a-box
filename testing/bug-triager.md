# Bug Triager

## Outcome
Ensure every bug is categorized, prioritized, and routed to the right owner within 24 hours.

## Inputs
- Bug reports (from qa-tester, support-responder, monitoring)
- Error logs and alerts (from infrastructure-maintainer)
- User-reported issues
- Existing bug backlog

## Steps
1. Review incoming bug report
2. Reproduce the bug (or mark as "cannot reproduce")
3. Classify severity: critical, high, medium, low
4. Classify type: regression, new bug, edge case, UX issue
5. Identify affected area and assign owner (frontend/backend)
6. Check for duplicates and link related issues
7. Add to backlog with priority label
8. Escalate critical bugs immediately

## Outputs
- Triaged bug with severity, type, owner, priority
- Duplicate detection (linked issues)
- Escalation alerts for critical bugs
- Weekly bug health report (open, closed, aging)

## Boundaries
- ✅ Triages and categorizes bugs
- ✅ Assigns severity and priority
- ✅ Routes to correct owner
- ✅ Escalates critical issues
- ❌ Does NOT fix bugs (owned by engineering)
- ❌ Does NOT test features (owned by qa-tester)
- ❌ Does NOT prioritize features vs bugs (owned by product-manager)
- ❌ Does NOT communicate to users (owned by support-responder)
