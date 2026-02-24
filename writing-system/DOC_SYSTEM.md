# Document Writing System

## 1) Purpose
This system standardizes how humans and AI agents co-create high-quality documents. It defines:
- quality standards
- writing style defaults
- structure discipline
- revision rules

It is designed to be reused across document types (white papers, memos, articles, strategy docs, playbooks).

## 2) Core Principles
- AI amplifies clarity, speed, and structure.
- Humans retain judgment, prioritization, and final accountability.
- Content quality comes before wording polish.
- Structure is document-specific; quality standards are system-wide.
- Claims should be grounded, not inflated.

## 2.1) Context Modes (Workflow Router)
Use one of two context modes before intake:

- **Document-First Mode**: the primary purpose of the project is to write a document.
- **Project-Embedded Mode**: writing is one workstream inside an existing project.

Mode selection changes intake depth and drafting behavior:
- Document-First: full intake, full voice calibration, outline-first by default.
- Project-Embedded: lean intake, project context first, faster decision-oriented drafting.

## 3) Default Writing Style
Use this style unless the human asks for overrides.

- Tone: strategic, clear, premium, grounded.
- Voice: confident without hype.
- Clarity: explicit cause-effect logic; avoid vague abstraction.
- Readability: balanced sentence length; avoid dense blocks with too many ideas.
- Language: precise and practical; avoid buzzwords and generic consulting jargon.
- Framing: always make AI/human accountability explicit where relevant.

## 4) Style Override Policy
The default style applies by default.

For each document, the agent must:
1. briefly restate the default style in 2-4 bullets
2. ask whether any style overrides are needed
3. apply overrides only after confirmation

Example override areas:
- tone (more executive, more instructional, more narrative)
- sentence length (shorter or denser)
- terminology (technical or simplified)
- formatting density

## 5) Voice Calibration Policy
Voice calibration defaults to required in Document-First mode and optional in Project-Embedded mode.

Before drafting, request 3-5 writing samples from the human, ideally from the same document type as the target output.

The agent should infer and confirm:
- typical sentence structure and length
- vocabulary preferences and word choices
- information organization and transition style
- formatting patterns (headings, bullets, spacing)
- storytelling vs direct instruction balance

If calibrated voice conflicts with system defaults:
- keep clarity and non-hype standards
- adapt phrasing and rhythm to the human voice
- ask one explicit clarification if the conflict is material

For Project-Embedded mode:
- skip calibration when speed is the priority and existing project docs already establish tone
- run a lightweight calibration only if the human asks for style matching

## 6) Document Blueprint Rules
Every document must lock these items before drafting:
- objective
- audience
- decision/action the document should enable
- non-negotiable key messages
- scope boundaries (in scope and out of scope)
- required sections for that specific document type

## 7) Quality Checklist (Final Gate)
A document is final only if all are true:
- key messages are accurately captured
- section flow supports decision-making
- writing is clear, concise, and non-repetitive
- wording matches agreed style/voice
- AI/human accountability is explicit where needed
- terminology is consistent end-to-end

## 8) Revision Protocol
Use this structure for feedback:
- Section
- Keep
- Change
- Replace with (optional)
- Rule to remember

Use explicit decisions:
- Accept: [items]
- Reject: [items]

Agent must apply accepted changes only, then summarize what changed.
