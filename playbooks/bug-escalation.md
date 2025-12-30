# Playbook: Bug Escalation

## When to Use
- Critical bug affecting >5% users
- Security vulnerability
- Data loss or corruption
- Payment/billing issues
- Complete feature breakage

## Pipeline

```
[DETECTION]
→ support-responder OR infrastructure-maintainer (detect)
→ bug-triager (classify severity)

[CRITICAL PATH - if severity = critical]
→ bug-triager (escalate immediately)
→ delivery-manager (coordinate response)
→ backend-architect OR frontend-developer (diagnose + fix)
→ code-reviewer (expedited review)
→ qa-tester (verify fix)
→ infrastructure-maintainer (hotfix deploy)

[COMMUNICATION]
→ support-responder (customer communication)
→ release-retrospective-owner (post-mortem)
```

## Severity Definitions

| Severity | Definition | Response Time | Examples |
|----------|------------|---------------|----------|
| Critical | System down, data loss, security breach | <1 hour | Payment failing, auth broken, data leak |
| High | Major feature broken, significant user impact | <4 hours | Core workflow broken, >20% users affected |
| Medium | Feature degraded, workaround exists | <24 hours | Slow performance, UI glitch |
| Low | Minor issue, cosmetic | Next sprint | Typo, alignment issue |

## Escalation Matrix

| Severity | Who to Alert | Channel |
|----------|--------------|---------|
| Critical | Founder + Engineering Lead | Phone/SMS |
| High | Engineering Lead | Slack urgent |
| Medium | Team Lead | Slack |
| Low | Backlog | Ticket system |

## Incident Response Template

```markdown
## Incident: [TITLE]
Severity: [CRITICAL/HIGH]
Detected: [TIMESTAMP]
Resolved: [TIMESTAMP]
Duration: [X hours]

### Impact
- Users affected: [number/%]
- Revenue impact: [if applicable]
- Data impact: [if applicable]

### Timeline
- [TIME] - Issue detected by [who]
- [TIME] - Escalated to [who]
- [TIME] - Root cause identified
- [TIME] - Fix deployed
- [TIME] - Confirmed resolved

### Root Cause
[What actually caused the issue]

### Fix
[What was done to resolve]

### Prevention
[What will prevent recurrence]
- [ ] Action item 1 - Owner - Deadline
- [ ] Action item 2 - Owner - Deadline
```

## Post-Mortem Required
- All Critical incidents: within 48 hours
- High incidents with >4 hour resolution: within 1 week
