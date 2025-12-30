![Visitors](https://hits.sh/github.com/fom-dev/company-in-a-box.svg?style=flat-square&label=visitors&color=5BDC9E)

# AI Company OS

A complete organizational structure for running a software house using AI agents. Each agent has a single, clear responsibility with defined inputs, outputs, and boundaries.

## Philosophy

- **One agent = one repeatable job**
- **If work piles up → create a new agent**
- **If a process repeats 3x → create a playbook**
- **Strict boundaries prevent chaos**

This is not a general-purpose AI assistant. It's a structured organization where every role has clear ownership.

## Quick Start

1. Clone this repo
2. Pick a playbook for what you're trying to do (e.g., `playbooks/product-launch.md`)
3. Follow the pipeline, invoking each agent in sequence
4. Each agent file tells you exactly what inputs it needs and what outputs it produces

## Structure

```
├── client-management/    # Client relationships and scope
├── design/               # UX research and UI design
├── engineering/          # Build and ship code
├── legal/                # Contracts, IP, NDAs
├── marketing/            # Growth and content
├── operations/           # Finance, support, knowledge
├── playbooks/            # End-to-end workflows
├── product/              # Requirements and prioritization
├── project-management/   # Delivery and coordination
├── sales/                # Lead gen to close
├── security/             # Protection and compliance
└── testing/              # QA and bug management
```

## Agents (42 total)

See [AGENTS.md](AGENTS.md) for the complete index with descriptions.

## Playbooks (10 total)

| Playbook | Use Case |
|----------|----------|
| [product-launch](playbooks/product-launch.md) | Ship a new product or major feature |
| [sprint-execution](playbooks/sprint-execution.md) | Run a development sprint |
| [growth-experiment](playbooks/growth-experiment.md) | Test marketing hypotheses |
| [content-campaign](playbooks/content-campaign.md) | Create and distribute content |
| [bug-escalation](playbooks/bug-escalation.md) | Handle critical bugs |
| [client-onboarding](playbooks/client-onboarding.md) | Onboard new clients |
| [sales-pipeline](playbooks/sales-pipeline.md) | Acquire new clients |
| [scope-change](playbooks/scope-change.md) | Handle scope changes |
| [security-incident](playbooks/security-incident.md) | Respond to security issues |
| [project-handoff](playbooks/project-handoff.md) | Transfer project ownership |

## Agent File Format

Every agent follows this structure:

```markdown
# Agent Name

## Outcome
A clear, verifiable result this agent produces.

## Inputs
- What the agent receives
- In what format

## Steps
1. Explicit operational steps
2. No creativity outside the role
3. No decisions outside authority

## Outputs
- Final deliverables
- Ready for other agents to consume

## Boundaries
- ✅ What this agent does
- ❌ What this agent does NOT do (and who owns it)
```

## How to Use

### With AI Tools
Feed the relevant agent file(s) into your AI tool as context. The agent definition provides:
- Clear scope (what to do)
- Guardrails (what not to do)
- Expected output format

### As Team Documentation
Use these definitions to:
- Clarify role responsibilities
- Onboard new team members
- Identify gaps in your organization
- Create job descriptions

### Building Workflows
Chain agents using playbooks:

```
product-manager (requirements)
→ estimator (effort)
→ sprint-planner (scope)
→ engineering (build)
→ qa-tester (validate)
→ infrastructure-maintainer (deploy)
```

## Customization

### Adding Agents
1. Identify a pile of work with no clear owner
2. Create a file in the appropriate department
3. Follow the standard format
4. Define boundaries clearly (especially what the agent does NOT do)

### Adding Playbooks
1. Notice a multi-step process you repeat
2. Map the pipeline (which agents, in what order)
3. Add checkpoints and templates
4. Include decision criteria

### Removing Agents
If an agent isn't being used:
1. Check if another agent absorbed its work
2. If yes, update that agent's boundaries
3. Delete the unused agent file

## Principles

1. **Single Responsibility**: One agent, one outcome
2. **Clear Boundaries**: Every agent knows what it does NOT do
3. **Explicit Handoffs**: Outputs from one agent are inputs to another
4. **No Heroics**: If an agent can't do something, it routes to the right owner
5. **Documentation as Code**: Agent definitions are the source of truth

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## License

Apache 2.0 - see [LICENSE](LICENSE)
