# Playbook: Sprint Execution

## When to Use
- Every sprint (1-2 week cycles)
- Standard delivery cadence

## Pipeline

```
[PLANNING]
→ product-manager (prioritized backlog)
→ sprint-planner (scope sprint)
→ delivery-manager (confirm capacity)

[EXECUTION]
→ delivery-manager (daily tracking)
→ priority-arbiter (if conflicts arise)
→ [BUILD]
   → backend-architect + frontend-developer
   → code-reviewer (PR reviews)
   → qa-tester (testing)
   → bug-triager (issues)

[CLOSE]
→ infrastructure-maintainer (deploy)
→ delivery-manager (sprint report)
→ release-retrospective-owner (retro)
→ sprint-planner (next sprint)
```

## Sprint Ceremonies

| Ceremony | When | Duration | Owner | Attendees |
|----------|------|----------|-------|-----------|
| Sprint Planning | Day 1 | 1-2 hours | sprint-planner | Product, Eng, Design |
| Daily Standup | Daily | 15 min | delivery-manager | Eng team |
| Backlog Grooming | Mid-sprint | 1 hour | product-manager | Product, Eng |
| Sprint Review | Last day | 30 min | delivery-manager | All stakeholders |
| Retrospective | Last day | 45 min | release-retrospective-owner | Sprint team |

## Daily Standup Format

Each team member answers:
1. What did I complete since last standup?
2. What will I work on today?
3. Any blockers?

Async alternative: Post in Slack by 10am.

## Sprint Health Indicators

| Indicator | Green | Yellow | Red |
|-----------|-------|--------|-----|
| Burndown | On track | 1-2 days behind | >2 days behind |
| Blockers | 0 | 1-2 (being resolved) | >2 or unresolved |
| Scope | Frozen | Minor clarifications | Scope creep |
| Team | Focused | Some context switching | Fire fighting |

## End of Sprint Checklist

- [ ] All committed items done or explicitly carried over
- [ ] PRs merged and deployed to staging
- [ ] QA sign-off on completed items
- [ ] Demo ready for sprint review
- [ ] Carry-over items documented with reason
- [ ] Retrospective scheduled
- [ ] Next sprint planned

## Carry-Over Rules
- Max 20% carry-over acceptable
- >20% triggers process review
- Same item carried over 2x = escalate to product-manager
