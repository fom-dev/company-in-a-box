# Playbook: Scope Change

## When to Use
- Client requests work outside original SOW
- Requirements change mid-project
- New features or functionality requested
- Timeline change requested

## Pipeline

```
[REQUEST]
→ client-manager (receive and document)
→ scope-change-handler (classify and assess)

[ESTIMATE]
→ product-manager (requirements clarity)
→ backend-architect / frontend-developer (effort estimate)
→ delivery-manager (timeline impact)
→ finance-tracker (budget impact)

[DECISION]
→ scope-change-handler (prepare change order)
→ client-manager (present to client)
→ contract-reviewer (if terms affected)

[APPROVAL]
→ client-manager (get client sign-off)
→ scope-change-handler (document approval)

[IMPLEMENT]
→ sprint-planner (add to backlog)
→ delivery-manager (update project plan)
→ client-manager (confirm timeline)
```

## Change Classification

| Type | Definition | Process | Billing |
|------|------------|---------|---------|
| Clarification | Within original intent | Document only | No charge |
| Minor Change | <8 hours effort | Quick approval | Absorb or bill per contract |
| Major Change | >8 hours effort | Full change order | Always billable |
| Scope Reduction | Removing work | Document credit | Possible credit |

## Change Request Template

```markdown
## Change Request: CR-[NUMBER]
Date: [DATE]
Requested By: [CLIENT NAME]
Project: [PROJECT NAME]

### Description
[What is being requested]

### Reason
[Why this change is needed]

### Impact Assessment
- Effort: [X hours/days]
- Timeline: [Impact on milestones]
- Cost: [Additional investment]
- Risk: [Any new risks introduced]

### Options
1. [Option A with tradeoffs]
2. [Option B with tradeoffs]
3. [Decline and rationale]

### Recommendation
[Our recommended approach]

### Approval
- [ ] Client approval (signature/email)
- [ ] Date approved
- [ ] Updated SOW (if required)
```

## Client Communication Script

```markdown
"Thank you for sharing this requirement. To make sure we deliver 
exactly what you need, I'd like to walk you through the impact:

- This change would require approximately [X] additional hours
- It would affect the timeline by [Y]
- The additional investment would be [Z]

We have a few options:
1. [Option with full scope]
2. [Option with reduced scope]
3. [Option to defer]

What would work best for your priorities?"
```

## Escalation Triggers
- Client disputes change is out of scope
- Change >20% of original project value
- Change affects contractual commitments
- Client requests change without budget
- Multiple changes indicating scope creep pattern

## Red Flags
- "I thought this was included" (misaligned expectations)
- Frequent small changes (scope creep)
- Changes without clear owner (client-side confusion)
- Urgent changes with no budget discussion
