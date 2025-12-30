# Playbook: Product Launch

## When to Use
- Launching a new product
- Launching a major feature (changes user workflow)
- Public beta release

## Pipeline

```
opportunity-evaluator (go/no-go)
→ vision-keeper (alignment check)
→ product-manager (requirements)
→ launch-strategist (launch plan)
→ sprint-planner (scope sprints)
→ [BUILD PHASE]
   → ux-researcher → ui-designer
   → backend-architect → frontend-developer
   → code-reviewer → qa-tester
→ delivery-manager (track progress)
→ [MARKETING PHASE]
   → tiktok-strategist (angles/hooks)
   → content-creator (content)
   → distribution-manager (publish)
→ infrastructure-maintainer (deploy)
→ [POST-LAUNCH]
   → analytics-reporter (metrics)
   → experiment-tracker (log tests)
   → test-results-analyzer (analyze)
   → feedback-synthesizer (user feedback)
   → release-retrospective-owner (retro)
```

## Checkpoints

| Checkpoint | Owner | Gate Criteria |
|------------|-------|---------------|
| Go/No-Go | opportunity-evaluator | Strategic fit confirmed |
| Requirements Locked | product-manager | PRD approved, scope frozen |
| Design Complete | ui-designer | All screens, all states |
| Code Complete | frontend-developer + backend-architect | PR merged, tests passing |
| QA Sign-off | qa-tester | All critical tests pass |
| Launch Ready | launch-strategist | All assets ready, team aligned |
| Go Live | infrastructure-maintainer | Deployed, monitoring active |

## Success Metrics
- Day 1 signups
- Week 1 activation rate
- Day 7 retention
- NPS post-launch

## Rollback Criteria
- Error rate >5%
- Conversion drop >20%
- Critical bug affecting >10% users
