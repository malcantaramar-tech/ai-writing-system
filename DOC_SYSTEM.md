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
- Readability: favor connected argument flow over fragmented punch lines; use short sentences sparingly and intentionally for emphasis only.
- Rhythm: default to medium-length, logically linked sentences; vary length to maintain cadence without sounding abrupt or simplistic.
- Language: precise and practical; avoid buzzwords and generic consulting jargon.
- Person: avoid second person (you, your); use third person or institutional phrasing (organizations, leadership teams, the reader) unless the document type explicitly requires direct address.
- Punctuation: prefer commas (with conjunctions as needed) over semicolons when linking related clauses, unless the human requests otherwise.
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

## 6) Introduction Structure
Introductions should:
- Open with one or more context-setting paragraphs (market, situation, stakes). Do not start by describing the document the reader is about to read.
- End the first paragraph (or context block) with a sentence that cites or supports the context, e.g. “Key industry reports from [sources] already support this reading of the market.” Do not embed source citations in the middle of the opening context.
- Convey the key message of the document early (what the reader should take away).
- Include a brief closing paragraph or sentence that explains in 1–2 sentences what the document contains (roadmap).
- Call to action may be placed in the introduction when the document aims to prompt a decision or engagement.

## 7) Referencing External Sources
When the document cites external reports or research:
- Frame sources as reinforcing the document’s position, not as a summary of the source. Link to the report where possible.
- In the body, cite only the primary sources (e.g. 2–3 key reports) that directly support the argument. Place report references at the end of the relevant paragraph when they support context (e.g. “Key industry reports from X, Y, Z support this view.”).
- An optional **Sources** section at the end may list additional relevant reports (with links and one-line descriptions) for further reading, without citing them all in the body.

## 8) Document Blueprint Rules
Every document must lock these items before drafting:
- objective
- audience
- author (who is named as author of the document)
- decision/action the document should enable
- non-negotiable key messages
- scope boundaries (in scope and out of scope)
- required sections for that specific document type
- (Optional) reference document for header and section structure (e.g. Title | Subtitle, Last Updated, Author, Purpose, Status; numbered sections 0 | Introduction, 1 | …, etc.)

## 9) Quality Checklist (Final Gate)
A document is final only if all are true:
- key messages are accurately captured
- section flow supports decision-making
- writing is clear, concise, and non-repetitive
- wording matches agreed style/voice
- AI/human accountability is explicit where needed
- terminology is consistent end-to-end

## 10) Revision Protocol
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
