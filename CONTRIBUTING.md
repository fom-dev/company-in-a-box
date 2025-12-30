# Contributing

Thank you for considering contributing to AI Company OS.

## How to Contribute

### Adding New Agents

1. **Identify the need**: Is there a repeatable job without a clear owner?
2. **Choose the right department**: Where does this agent logically belong?
3. **Follow the format**: Use the standard agent template below
4. **Define boundaries clearly**: What does this agent NOT do?
5. **Update AGENTS.md**: Add your new agent to the index

### Agent Template

```markdown
# Agent Name

## Outcome
[Single sentence: what verifiable result does this agent produce?]

## Inputs
- [What the agent receives]
- [In what format]

## Steps
1. [First step]
2. [Second step]
3. [Continue until complete]

## Outputs
- [What the agent delivers]
- [Ready for other agents to consume]

## Boundaries
- ✅ [What this agent does]
- ✅ [What this agent does]
- ❌ Does NOT [action] (owned by [other-agent])
- ❌ Does NOT [action] (owned by [other-agent])
```

### Adding New Playbooks

1. **Identify the workflow**: Is this a multi-step process that repeats?
2. **Map the pipeline**: Which agents, in what order?
3. **Add checkpoints**: Where are the go/no-go decisions?
4. **Include templates**: What documents does this playbook produce?
5. **Update README.md**: Add your playbook to the table

### Playbook Template

```markdown
# Playbook: [Name]

## When to Use
- [Trigger condition 1]
- [Trigger condition 2]

## Pipeline

\`\`\`
[agent-1] (action)
→ [agent-2] (action)
→ [agent-3] (action)
\`\`\`

## Checkpoints

| Checkpoint | Owner | Gate Criteria |
|------------|-------|---------------|
| | | |

## Templates

[Include any templates this playbook uses]

## Checklist

- [ ] [Step 1]
- [ ] [Step 2]
```

## Guidelines

### Do
- Keep agents focused on a single outcome
- Define clear boundaries (what agent does NOT do)
- Specify which agent owns work this agent doesn't do
- Use concrete, measurable outcomes
- Include practical steps, not abstract principles

### Don't
- Create agents that overlap significantly
- Leave boundaries vague
- Add agents for one-time tasks
- Create agents without clear outputs
- Skip the "does NOT do" section

## Pull Request Process

1. Create a branch: `feature/agent-name` or `playbook/playbook-name`
2. Add your agent or playbook following the templates
3. Update AGENTS.md or README.md as needed
4. Submit PR with clear description of what this agent/playbook does
5. Respond to review feedback

## Questions?

Open an issue if you're unsure whether something should be:
- A new agent
- Added to an existing agent
- A playbook
- Something else entirely
