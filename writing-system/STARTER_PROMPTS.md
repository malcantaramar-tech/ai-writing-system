# Starter Prompts

Use these prompts to activate the writing system in Cursor.

## 1) Standard Starter (recommended default)

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

## 2) Document-First Mode

```text
Use the writing system files in writing-system/.
Context mode: Document-First.

Run full intake and required voice calibration.
Ask for 3-5 writing samples from the same document type.
Do not draft yet.

Return a pre-draft package for approval:
- objective
- audience
- decision/action enabled
- locked key messages
- proposed structure
- inferred voice profile
- drafting plan by section
```

## 3) Project-Embedded Mode

```text
Use the writing system files in writing-system/.
Context mode: Project-Embedded.

Run lean intake, prioritize existing project constraints and locked decisions, and skip voice calibration unless I request it.
Do not draft yet.

Return:
- decision-oriented structure
- key messages
- assumptions and constraints
- concise drafting plan
```

## 4) Existing Draft Revision

```text
Use the writing system files in writing-system/.
I already have a draft.

Do not rewrite everything.
First, assess structure, clarity, repetition, and message fidelity.
Then propose a focused revision plan with numbered changes.
Wait for my Accept/Reject before applying edits.
```

## 5) Final QA Pass

```text
Run a final quality check using writing-system/DOC_SYSTEM.md.

Validate:
- key message fidelity
- structure coherence
- clarity and non-repetition
- terminology consistency
- AI/human accountability clarity

Return:
1) issues found
2) suggested fixes
3) final readiness assessment
```
