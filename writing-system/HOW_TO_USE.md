# How to Use the Writing System

This writing system enables humans and AI agents to produce clear, high-quality documents faster by standardizing context intake, drafting flow, and revision quality.

It guides you through voice calibration, proposes a default writing style you can adjust, and runs structured intake so the agent has the right context before drafting. It also supports guided feedback cycles, so your comments are captured in a format the agent can apply quickly and consistently until the document reaches a final version.

## Key Steps

### Step 1: Add the system files to your project
Copy these files into your local project folder:
- `writing-system/DOC_SYSTEM.md`
- `writing-system/INTAKE_QUESTIONNAIRE.md`
- `writing-system/AGENT_PROMPT_TEMPLATE.md`

You can use this in:
- a writing-only project
- an existing project where writing is one workstream

### Step 2: Open Cursor and paste the starter prompt
Use the prompt below to activate the system.

After Step 2, the remaining workflow runs in Cursor and is led by the agent. The agent will select the right mode (Document-First or Project-Embedded), run structured intake, calibrate style when needed, propose a pre-draft package for approval, draft the document, and support revision cycles with explicit accept/reject decisions.

## Starter Prompt

```text
Use the writing system in this project:
- writing-system/DOC_SYSTEM.md
- writing-system/INTAKE_QUESTIONNAIRE.md
- writing-system/AGENT_PROMPT_TEMPLATE.md

Start by selecting context mode (Document-First or Project-Embedded), then run intake in order.
Do not draft yet.

After intake, return:
1) objective
2) audience
3) decision/action enabled
4) locked key messages
5) proposed structure
6) inferred voice profile
7) mode-specific drafting plan

Wait for my approval before drafting.
```
