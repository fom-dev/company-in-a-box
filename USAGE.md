# Usage Guide

This framework is not software to install—it's a structured set of prompts and workflows to use with AI assistants like Claude.

## Quick Start

### 1. Use a Single Agent

Copy the agent file content and paste it into your AI assistant, then give it a task.

**Example with `content-creator`:**

```
[Paste content of marketing/content-creator.md]

Now write a LinkedIn post announcing our new UML diagram tool. 
Target audience: software developers and tech leads.
Key benefit: 10x faster than traditional tools.
```

### 2. Use a Playbook

Playbooks chain multiple agents together. Follow the pipeline step by step.

**Example with `product-launch`:**

```
[Paste content of playbooks/product-launch.md]

I'm launching a SaaS UML tool in 2 weeks. 
Guide me through this playbook step by step.
```

## Usage Methods

### Claude.ai (Web/App)

1. Open a new conversation
2. Copy/paste the agent or playbook content
3. Describe your task
4. Claude will follow the agent's structure

### Claude Code (Terminal)

```bash
cd company-in-a-box

# Ask Claude to read and use an agent
claude "Read marketing/content-creator.md and act as that agent. Write a Twitter thread about our new feature."

# Or use a playbook
claude "Read playbooks/sprint-execution.md and help me plan next sprint. Here's our backlog: ..."
```

### API / System Prompt

Include the agent definition in your system prompt:

```python
system_prompt = """
You are an AI assistant acting as the following agent:

[Content of agent file]

Follow the agent's steps, respect boundaries, and produce the specified outputs.
"""
```

## Practical Examples

### Example 1: Get Marketing Content

**Agent:** `marketing/content-creator.md`

```
Act as the content-creator agent.

Inputs:
- Brief: Launch announcement for "FlowUML"
- Target: Software developers, CTOs
- Channel: LinkedIn
- Key benefit: AI-powered diagram generation

Produce the outputs specified in the agent definition.
```

### Example 2: Handle a Bug

**Playbook:** `playbooks/bug-escalation.md`

```
Act as my bug-triager following the bug-escalation playbook.

A user reported: "App crashes when exporting large diagrams to PDF. 
Happens every time with files over 50 elements. Started after last update."

Triage this bug and tell me what to do.
```

### Example 3: Plan a Sprint

**Agents:** `product/sprint-planner.md` + `project-management/delivery-manager.md`

```
First, act as sprint-planner:

Our backlog:
1. User authentication (8 points)
2. Export to PNG (3 points)
3. Fix alignment bug (2 points)
4. Dark mode (5 points)
5. Team collaboration (13 points)

Team capacity: 18 points
Carry-over: none

Plan the sprint.
```

### Example 4: Scope Change Request

**Playbook:** `playbooks/scope-change.md`

```
Follow the scope-change playbook.

Client request: "We need to add real-time collaboration to the MVP."

Original scope: Single-user diagram editor
Current phase: Week 3 of 8
Budget: Fixed price

Help me handle this.
```

### Example 5: Chain Multiple Agents

Run a full pipeline manually:

```
Step 1 - Act as tiktok-strategist:
"Our product is an AI UML tool. Give me 3 angles and hooks for TikTok."

Step 2 - Act as content-creator:
"Take angle #2 from above and write a full TikTok script."

Step 3 - Act as analytics-reporter:
"This content got 50K views, 2K likes, 100 comments, 500 profile visits, 50 signups. Analyze and recommend next steps."
```

## Tips

### Be Specific with Inputs
Agents work best when you provide all the inputs listed in their definition.

### Respect Boundaries
If an agent says "Does NOT do X", don't ask it to do X. Use the right agent for the job.

### Use Playbooks for Complex Tasks
Single agents handle single jobs. Playbooks coordinate multiple agents for end-to-end workflows.

### Customize Agents
Fork the repo and modify agents to match your company's specific processes, tools, and terminology.

## File Structure Reference

```
company-in-a-box/
├── [department]/
│   └── [agent].md          # Agent definitions
├── playbooks/
│   └── [workflow].md       # Multi-agent workflows
├── AGENTS.md               # Full agent index
└── USAGE.md                # This file
```

## Need Help?

- Check `AGENTS.md` for the full list of available agents
- Check `README.md` for the philosophy and structure
- Open an issue for questions or suggestions