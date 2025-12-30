# Playbook: Growth Experiment

## When to Use
- Testing new marketing angles
- A/B testing landing pages
- Testing pricing changes
- Testing new channels
- Any hypothesis that needs validation

## Pipeline

```
[HYPOTHESIS]
→ product-manager or tiktok-strategist (define hypothesis)
→ opportunity-evaluator (worth testing?)
→ experiment-tracker (log experiment)

[BUILD VARIANT]
→ content-creator (if content test)
→ frontend-developer (if product test)
→ qa-tester (verify tracking works)

[RUN]
→ distribution-manager (launch variant)
→ experiment-tracker (monitor status)
→ analytics-reporter (collect data)

[ANALYZE]
→ test-results-analyzer (determine winner)
→ experiment-tracker (record results)

[ACT]
→ product-manager (decide: scale, iterate, kill)
→ [if scale] → relevant team implements winner
```

## Experiment Brief Template

```markdown
## Experiment: [NAME]
ID: EXP-[NUMBER]
Owner: [NAME]
Start Date: [DATE]
Duration: [X days/weeks]

### Hypothesis
If we [CHANGE], then [METRIC] will [IMPROVE/DECREASE] by [X%]
because [REASONING].

### Variants
- Control: [description]
- Variant A: [description]
- Variant B: [description] (optional)

### Success Metric
Primary: [metric + target]
Secondary: [guardrail metrics]

### Sample Size
Minimum: [number] per variant
Estimated duration: [days]

### Risks
- [risk 1]
- [risk 2]
```

## Minimum Requirements
- Clear hypothesis (falsifiable)
- Single primary metric
- Minimum 1 week runtime
- Statistical significance >90% to declare winner
- No conflicting experiments on same audience

## Decision Framework
| Result | Confidence | Action |
|--------|------------|--------|
| Winner | >95% | Scale immediately |
| Winner | 90-95% | Scale with monitoring |
| Inconclusive | - | Extend test or redesign |
| Loser | >90% | Kill variant |
