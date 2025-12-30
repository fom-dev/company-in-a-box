# Playbook: Sales Pipeline

## When to Use
- Standard B2B sales process
- New client acquisition
- Expansion with existing clients

## Pipeline

```
[LEAD GENERATION]
→ sales-developer (prospecting)
→ content-creator (sales enablement content)

[QUALIFICATION]
→ sales-developer (BANT qualification)
→ account-executive (discovery call)

[PROPOSAL]
→ account-executive (scope discussion)
→ backend-architect + frontend-developer (effort estimate)
→ delivery-manager (capacity check)
→ proposal-writer (proposal document)
→ contract-reviewer (terms review)

[NEGOTIATION]
→ account-executive (negotiation)
→ contract-reviewer (contract review)
→ nda-manager (NDA if needed)

[CLOSE]
→ account-executive (close deal)
→ contract-reviewer (final contract)
→ client-manager (handoff)
```

## Sales Stages

| Stage | Definition | Exit Criteria | Owner |
|-------|------------|---------------|-------|
| Lead | Identified potential | Contact info verified | sales-developer |
| Qualified | BANT confirmed | Discovery call scheduled | sales-developer |
| Discovery | Needs understood | Requirements documented | account-executive |
| Proposal | Solution presented | Proposal delivered | account-executive |
| Negotiation | Terms discussed | Agreement on scope/price | account-executive |
| Contract | Legal review | Contract signed | account-executive |
| Won/Lost | Deal closed | Handoff complete or loss documented | account-executive |

## BANT Qualification

```markdown
## Budget
- [ ] Has budget allocated for this type of project
- [ ] Budget range aligns with our minimum engagement
- [ ] Decision maker controls budget

## Authority
- [ ] Decision maker identified
- [ ] Decision maker engaged in process
- [ ] Buying process understood

## Need
- [ ] Clear problem articulated
- [ ] Problem is priority for organization
- [ ] Our solution fits the need

## Timeline
- [ ] Project has defined timeline
- [ ] Timeline is realistic
- [ ] No blockers to starting
```

## Discovery Call Template

```markdown
### Opening (5 min)
- Introductions
- Agenda confirmation

### Understanding (20 min)
- What prompted this conversation?
- What problem are you trying to solve?
- What have you tried before?
- What does success look like?
- What's the impact if this isn't solved?

### Solution Discussion (15 min)
- How we've solved similar problems
- Relevant case study
- High-level approach

### Logistics (10 min)
- Timeline expectations
- Budget range
- Decision process
- Next steps

### Wrap-up (5 min)
- Summary of understanding
- Agreed next steps
- Follow-up timeline
```

## Win/Loss Analysis

After every closed deal (won or lost):

```markdown
## Deal: [Client Name]
Outcome: [Won/Lost]
Deal Size: [Amount]
Sales Cycle: [Days]

### If Won
- Primary reason won:
- Competitive situation:
- What we did well:
- What we could improve:

### If Lost
- Primary reason lost:
- Who did they choose:
- What we could have done differently:
- Should we re-engage later: [Yes/No]
```
