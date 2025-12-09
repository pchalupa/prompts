# Prompts&Agents
This repository contains a collection of custom prompts and agents designed to enhance the capabilities of AI models in various tasks. Each prompt or agent is tailored for specific use cases, ranging from technical documentation to creative writing.

## Useful Links
- [Custom agent file structure](https://code.visualstudio.com/docs/copilot/customization/custom-agents#_custom-agent-file-structure)
- [Example agent profiles](https://docs.github.com/en/copilot/how-tos/use-copilot-agents/coding-agent/create-custom-agents#example-agent-profiles)

## Agent Template

When creating a new agent, use the following template to ensure consistency:

```chatagent
---
name: 'agent-name'
description: 'Short description of the agent.'
tools: ['tool1', 'tool2']
model: Gemini 3 Pro (Preview) (copilot)
handoffs:
  - label: Action Label
    agent: target-agent
    prompt: Prompt for the target agent.
---
You are the **[agent-name]** agent. Your goal is [goal description].

## Responsibilities
- [Responsibility 1]
- [Responsibility 2]

## Process
1. **Step 1**: [Description]
2. **Step 2**: [Description]

## Output Guidelines
- [Guideline 1]
- [Guideline 2]
```

## Prompt Template

When creating a new prompt file (`.prompt.md`), use the following template:

```prompt
---
name: 'prompt-name'
description: 'Short description of what the prompt does.'
argument-hint: 'Optional hint for arguments'
tools: ['tool1', 'tool2']
model: Gemini 3 Pro (Preview) (copilot)
---
You are an expert [role]. Your goal is [goal description].

## Responsibilities
- [Responsibility 1]
- [Responsibility 2]

## Process
1. **Step 1**: [Description]
2. **Step 2**: [Description]

## Output Guidelines
- [Guideline 1]
- [Guideline 2]
```