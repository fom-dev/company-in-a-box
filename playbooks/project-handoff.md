# Playbook: Project Handoff

## When to Use
- Team member leaving project
- Team member leaving company
- Project transitioning between teams
- Client requesting new team
- Long-term maintenance handoff

## Pipeline

```
[PREPARE]
→ delivery-manager (identify handoff need)
→ knowledge-manager (audit documentation state)
→ outgoing owner (document tribal knowledge)

[DOCUMENT]
→ outgoing owner (create handoff document)
→ code-reviewer (code walkthrough)
→ infrastructure-maintainer (system access docs)

[TRANSFER]
→ access-controller (provision new team)
→ onboarding-coordinator (schedule knowledge transfer)
→ delivery-manager (overlap period)

[VALIDATE]
→ incoming owner (shadow and verify)
→ qa-tester (verify incoming can operate)
→ client-manager (introduce to client if applicable)

[COMPLETE]
→ access-controller (revoke outgoing access)
→ delivery-manager (confirm handoff complete)
→ release-retrospective-owner (handoff retro)
```

## Handoff Document Template

```markdown
# Project Handoff: [PROJECT NAME]
Date: [DATE]
From: [OUTGOING]
To: [INCOMING]

## Project Overview
- Client: [NAME]
- Start Date: [DATE]
- Current Phase: [PHASE]
- Contract End: [DATE]

## Key Contacts
| Role | Name | Email | Notes |
|------|------|-------|-------|
| Client Decision Maker | | | |
| Client Technical Lead | | | |
| Internal PM | | | |

## Technical Overview
### Architecture
[High-level architecture description]

### Tech Stack
- Frontend: [technologies]
- Backend: [technologies]
- Infrastructure: [hosting, services]
- Key integrations: [third-party services]

### Repositories
| Repo | URL | Purpose |
|------|-----|---------|
| | | |

### Environments
| Environment | URL | Access |
|-------------|-----|--------|
| Production | | |
| Staging | | |
| Development | | |

### Credentials & Secrets
[Location of credentials - NOT the credentials themselves]

## Current State
### In Progress
- [Current work items]

### Upcoming
- [Planned work]

### Known Issues
- [Open bugs or concerns]

### Technical Debt
- [Known shortcuts or issues to address]

## Processes
### Deployment
[How to deploy]

### Monitoring
[What to monitor, where alerts go]

### Support
[How support requests come in, SLAs]

## Tribal Knowledge
### Things That Aren't Obvious
- [Gotchas, quirks, historical decisions]

### Client Preferences
- [How client likes to communicate, pet peeves]

### What I Wish I Knew
- [Advice for incoming owner]

## Open Questions
- [Unresolved items incoming owner needs to handle]
```

## Knowledge Transfer Sessions

| Session | Duration | Attendees | Content |
|---------|----------|-----------|---------|
| Architecture Overview | 2 hours | Tech leads | System design, key decisions |
| Codebase Walkthrough | 2-4 hours | Developers | Code structure, patterns, gotchas |
| Client Relationship | 1 hour | Account/PM | History, preferences, politics |
| Operations | 1 hour | Ops/DevOps | Deployment, monitoring, incidents |
| Open Items | 1 hour | All | In-progress work, upcoming |

## Overlap Period Guidelines

| Handoff Type | Minimum Overlap |
|--------------|-----------------|
| Simple project | 3 days |
| Medium complexity | 1 week |
| Complex project | 2 weeks |
| Critical system | 4 weeks |

## Checklist

### Before Handoff
- [ ] Handoff document complete
- [ ] All documentation current
- [ ] Knowledge transfer sessions scheduled
- [ ] Incoming owner identified and available
- [ ] Client notified (if applicable)

### During Handoff
- [ ] Architecture walkthrough complete
- [ ] Codebase walkthrough complete
- [ ] Access provisioned for incoming
- [ ] Incoming shadows outgoing on live work
- [ ] Incoming completes task independently
- [ ] Client introduced to incoming (if applicable)

### After Handoff
- [ ] Outgoing access revoked
- [ ] Incoming confirmed as primary contact
- [ ] Support escalation updated
- [ ] Handoff retro completed
- [ ] Documentation updated with new owner

## Red Flags
- No overlap period possible
- Documentation severely outdated
- Single point of failure (only one person knows)
- Client relationship issues during transition
- Incoming overwhelmed or unclear

## Emergency Handoff
If outgoing unavailable (illness, sudden departure):
1. Identify most knowledgeable remaining team member
2. Audit all documentation immediately
3. Check all access and credentials
4. Contact client proactively
5. Extend timelines if needed
6. Document everything discovered
