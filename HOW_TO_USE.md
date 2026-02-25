# How to Use the Writing System

## (i) What exactly is this writing system?

This writing system is a shared set of rules and steps for co-creating documents with an AI agent. It defines what gets decided before any draft (objective, audience, author, key messages, scope, structure), how the agent should write by default (strategic, clear, grounded, with connected prose and no second person unless the document type requires it), and how feedback is given and applied so that revisions stay consistent and traceable.

The system is valuable because it reduces back-and-forth and rework. When the agent runs intake first, it has the right context from the start, so the first draft is closer to what the user needs. When voice and style are calibrated up front, the output matches the user’s tone and the document type. When revision follows a simple accept/reject protocol, the user and the agent stay aligned on what changed and what rules to carry forward. The result is faster, more predictable document quality across white papers, memos, strategy docs, playbooks, and similar artifacts.

---

## (ii) How can it be used?

The system can be used in two ways, depending on whether the main goal is to produce a single document or to support writing as one thread inside a larger project.

In **Document-First** mode, the project exists to write the document. The agent runs full intake (objective, audience, author, decision or action the document should enable, key messages, scope, sources, structure, voice calibration, style overrides, drafting mode), proposes an outline with section intent, and waits for approval before drafting. Voice calibration is required so the draft matches the user’s style.

In **Project-Embedded** mode, the document supports an existing project. The agent keeps intake lean and focused on decisions and constraints that are already fixed. Voice calibration is optional. The agent still returns a clear summary and a focused structure tied to project context before drafting.

In both modes, the user answers the intake questions in order (one at a time if the agent asks that way), reviews the pre-draft package (objective, audience, author, decision/action, locked messages, structure, voice profile, drafting plan), and approves or adjusts before any draft is written. After the draft, the user gives feedback in the agreed format (section, keep, change, replace with, rule to remember) and states what to accept and what to reject. The agent applies only accepted changes and summarizes what changed.

---

## (iii) How to get started

**1. Add the system files to the project**

Ensure these files are in the project (for example under a `writing-system/` folder or at the project root):

- `DOC_SYSTEM.md`
- `INTAKE_QUESTIONNAIRE.md`
- `AGENT_PROMPT_TEMPLATE.md`

The same files work for writing-only projects and for projects where writing is one workstream.

**2. Open Cursor and paste the starter prompt**

In a Cursor chat, paste the prompt below. The agent will use it to load the writing system, choose Document-First or Project-Embedded mode, and run the intake sequence in order without drafting until the user has approved the pre-draft package.

**3. Answer intake and approve before drafting**

The agent will ask for context step by step (objective, audience, author, decision/action, key messages, scope, sources, structure, voice samples if needed, style overrides, drafting mode). Once intake is complete, the agent returns a short package: objective, audience, author, decision/action enabled, locked key messages, proposed structure, inferred voice profile, and mode-specific drafting plan. The user reviews this and approves or asks for changes. Only after approval does the agent draft the document.

**4. Revise with accept/reject**

After the draft, the user gives feedback using the revision protocol (section, keep, change, replace with, rule to remember) and explicitly accepts or rejects each item. The agent applies only accepted changes and summarizes what changed.

---

## Starter prompt

Copy and paste this into Cursor to start a session with the writing system:

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
3) author
4) decision/action enabled
5) locked key messages
6) proposed structure
7) inferred voice profile
8) mode-specific drafting plan

Wait for my approval before drafting.
```
