# Playbook: Security Incident

## When to Use
- Suspected or confirmed security breach
- Data leak or exposure
- Unauthorized access detected
- Vulnerability actively exploited
- Client reports security concern

## Pipeline

```
[DETECT & TRIAGE]
→ incident-responder (confirm and classify)
→ security-auditor (initial assessment)

[CONTAIN]
→ incident-responder (isolate systems)
→ access-controller (revoke compromised credentials)
→ infrastructure-maintainer (system isolation)

[INVESTIGATE]
→ incident-responder (root cause analysis)
→ security-auditor (scope determination)
→ compliance-monitor (regulatory requirements)

[COMMUNICATE]
→ client-manager (affected clients)
→ legal → contract-reviewer (legal obligations)
→ support-responder (prepare for inquiries)

[RECOVER]
→ infrastructure-maintainer (restore systems)
→ security-auditor (verify clean)
→ access-controller (new credentials)

[POST-INCIDENT]
→ incident-responder (post-mortem)
→ release-retrospective-owner (lessons learned)
→ compliance-monitor (regulatory reporting)
```

## Severity Classification

| Severity | Definition | Response |
|----------|------------|----------|
| SEV1 - Critical | Active breach, data exfiltration, system compromise | All hands, immediate |
| SEV2 - High | Confirmed vulnerability, potential exposure | 1 hour response |
| SEV3 - Medium | Suspicious activity, no confirmed impact | 4 hour response |
| SEV4 - Low | Minor security issue, no immediate risk | 24 hour response |

## Communication Matrix

| Audience | SEV1 | SEV2 | SEV3 | SEV4 |
|----------|------|------|------|------|
| Leadership | Immediate | 1 hour | Daily | Weekly |
| Affected Clients | <24 hours | <48 hours | If required | No |
| All Clients | If widespread | No | No | No |
| Regulators | Per requirements | Per requirements | No | No |
| Public | If required | No | No | No |

## Incident Log Template

```markdown
## Incident ID: SEC-[YYYY]-[NUMBER]
Severity: [SEV1/2/3/4]
Status: [ACTIVE/CONTAINED/RESOLVED/CLOSED]

### Timeline
| Time | Event | Action | Owner |
|------|-------|--------|-------|
| | | | |

### Impact Assessment
- Systems affected:
- Data affected:
- Users/clients affected:
- Business impact:

### Containment Actions
- [ ] Action 1
- [ ] Action 2

### Root Cause
[To be completed post-investigation]

### Remediation
[To be completed post-investigation]

### Notifications Sent
| Audience | Time | Method | Content |
|----------|------|--------|---------|
| | | | |
```

## Do NOT
- Destroy evidence (preserve logs)
- Communicate externally without legal review
- Speculate about cause or impact
- Promise anything to clients before facts known
- Resume normal operations before all-clear
